<template>
  <div>
  	<section>
		<h2><span>Contact</span></h2>
    <b-form @submit="onSubmit" @reset="onReset" v-if="show" class="container">
      <b-form-group 
                    label="Your Mail address:"
                    label-for="exampleInput1"
                    description="We'll never share your email with anyone else.">
        <b-form-input 
                      type="email"
                      v-model="form.email"
                      required
                      placeholder="Enter your email">
        </b-form-input>
      </b-form-group>
      <b-form-group id="exampleInputGroup2"
                    label="Your Name:"
                    label-for="exampleInput2">
        <b-form-input id="exampleInput2"
                      type="text"
                      v-model="form.title"
                      required
                      placeholder="Enter name">
        </b-form-input>
      </b-form-group>
        <b-form-group id="exampleInputGroup2"
                    label="Content:"
                    label-for="exampleInput2">
         <b-form-textarea id="textarea1"
                     v-model="form.content"
                     placeholder="Enter content"
                     :rows="3"
                     :max-rows="6">
    	</b-form-textarea>
      </b-form-group>
      <b-button type="submit" variant="secondly">Submit</b-button>
      <b-button type="reset" variant="secondly">Reset</b-button>
    </b-form>
    </section>
  </div>
</template>

<script>
export default {
  name:"Contact",
  data () {
    return {
      form: {
        email: '',
        title: '',
        content:'',
      },
      show: true
    }
  },
  methods: {
    onSubmit (evt) {
      evt.preventDefault();
      alert(JSON.stringify(this.form));
    },
    onReset (evt) {
      evt.preventDefault();
      /* Reset our form values */
      this.form.email = '';
      this.form.title = '';
      this.form.content =  '';
      /* Trick to reset/clear native browser form validation state */
      this.show = false;
      this.$nextTick(() => { this.show = true });
    }
  }
}
</script>
