<template>
  <div>
    <div class="row">
      <div class="col-md-6">
        <div class="form-group">
          <label for="name">Name</label>
          <input type="text" class="form-control" v-model="applicationForm.name" placeholder="Enter name">
        </div>
      </div>
      <div class="col-md-6">
        <div class="form-group">
          <label for="email">Email </label>
          <input type="email" class="form-control" v-model="applicationForm.email" placeholder="Enter email">
        </div>
      </div>
      <div class="col-md-6">
        <div class="form-group">
          <label for="">Programs of interest? </label>
          <input type="text" class="form-control" v-model="applicationForm.program_of_interest" placeholder="Enter email">
        </div>
      </div>
      <div class="col-md-6">
        <div class="form-group">
          <label for="email">Email </label>
          <input type="email" class="form-control" v-model="applicationForm.email" placeholder="Enter email">
        </div>
      </div>
      <div class="col-md-12">
        <div class="form-group">
          <label for="email" class="d-block">Which level are you working at?  </label>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="checkbox" id="inlineCheckbox1" value="option1">
            <label class="form-check-label" for="inlineCheckbox1">High School/Scedendary School</label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="checkbox" id="inlineCheckbox2" value="option2">
            <label class="form-check-label" for="inlineCheckbox2">Bachelors</label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="checkbox" id="inlineCheckbox3" value="option3">
            <label class="form-check-label" for="inlineCheckbox3">Others</label>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="form-group">
          <label for="">When  would you like to study at university?(required) </label>
          <input type="text" class="form-control"  placeholder="Type your answer">
        </div>
      </div>
      <div class="col-md-6">
        <div class="form-group">
          <label for="">Mailing Address </label>
          <input type="email" class="form-control"  placeholder="Type your answer">
        </div>
      </div>
      <div class="col-md-6">
        <div class="form-group">
          <label for="">Citizenship Status </label>
          <input type="text" class="form-control"  placeholder="Type your answer">
        </div>
      </div>
      <div class="col-md-6">
        <div class="form-group">
          <label for="">Emergency Contacts </label>
          <input type="text" class="form-control"  placeholder="Type your answer">
        </div>
      </div>
      <hr>
      <div class="col-md-12">
        <div class="form-group">
          <label for="email" class="d-block">Have you taken or plan to take ACT orSAT Exam? </label>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio1" value="option1">
            <label class="form-check-label" for="inlineRadio1">Yes</label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio2" value="option2">
            <label class="form-check-label" for="inlineRadio2">No</label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio3" value="option3" disabled>
            <label class="form-check-label" for="inlineRadio3">Planned</label>
          </div>
        </div>
      </div>
      <div class="col-md-12">
        <div class="form-group">
          <label for="email" class="d-block">If required will you be able to share your financial standing documents with us?</label>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio1" value="option1">
            <label class="form-check-label" for="inlineRadio1">Yes</label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio2" value="option2">
            <label class="form-check-label" for="inlineRadio2">No</label>
          </div>

        </div>
      </div>
      <div class="col-md-12">
        <div class="form-group">
          <label for="email" class="d-block">What is the source of your fundinds?</label>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio1" value="option1">
            <label class="form-check-label" for="inlineRadio1">Self-funding</label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio2" value="option2">
            <label class="form-check-label" for="inlineRadio2">Partialsupport</label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio2" value="option2">
            <label class="form-check-label" for="inlineRadio2">Employer support</label>
          </div>

        </div>
      </div>
      <div class="col-md-12">
        <div class="form-group">
          <label for="email" class="d-block">Specify your level of avilable funding per year so you can be matched with your best-fit university:</label>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio1" value="option1">
            <label class="form-check-label" for="inlineRadio1">$10,000- $20,000</label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio2" value="option2">
            <label class="form-check-label" for="inlineRadio2">$21,000 - $40,000</label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio2" value="option2">
            <label class="form-check-label" for="inlineRadio2">Abobe $40,000</label>
          </div>
        </div>
      </div>

    </div>

  </div>
</template>

<script>
export default {
  name: 'ApplicationForm',
  data() {
    return {
      applicationForm:{}
    }
  }

  }
</script>

