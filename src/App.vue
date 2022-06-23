<template>
  <div class="container">
    <button
        v-for="(tab,index) in tabs"
        :key="tab.name"
        @click="changeComponent(index)"
    >
      {{ tab.name }}
    </button>
    <component :is="selected" class="tab"></component>
  </div>
</template>

<script>

import Home from './components/Home.vue'
import About from './components/About.vue'
import ApplicationForm from './components/ApplicationForm.vue'

export default {
  name: 'App',
  data() {
    return {
      tabs: [
        {name: 'Home', component: 'Home'},
        {name: 'About', component: 'About'},
        {name: 'Application Form', component: 'ApplicationForm'},
      ],
      selected: 'Home',
    }
  },
  components: {
    Home,
    About,
    ApplicationForm
  },
  mounted() {
    this.changeComponent(0)
  },
  methods: {
    changeComponent(index) {
      console.log('index', index)
      this.selected = this.tabs[index].component;
      console.log('selected', this.selected)
    }
  }
}
</script>
