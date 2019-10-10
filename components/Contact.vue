<template>

  <section id="contact" class="section contact has-background-light">
    <div class="container" v-scroll-reveal.reset>
      <div class="content">
        <h4 class="cat-header has-text-centered is-full is-uppercase has-text-weight-semibold has-text-grey-dark">Contactez-moi</h4>
        <div class="columns is-centered">
          <div class="column is-two-fifths-desktop is-three-fifths-tablet is-full-mobile">

          <div v-if="errors.length" style="padding-bottom: 2rem; font-size: 0.95rem;">
            <ul>
              <div v-for="error in errors">
                <li>{{ error }}</li>
              </div>
            </ul>
          </div>

          <form name="contact" method="POST" netlify data-netlify="true" netlify-honeypot="bot-field" data-netlify-recaptcha="true">
          <input type="hidden" name="form-name" value="contact" />
            <b-field v-show="false" label="Bot Field" id="bot-field" name="bot-field">
              <b-input name="bot-field"></b-input>
            </b-field>

            <b-field label="Nom" id="namefield">
                <b-input v-model="name" name="name"></b-input>
            </b-field>

            <b-field label="Email">
                <b-input maxlength="30" v-model="email" name="email" @input="validateForm"></b-input>
            </b-field>

            <b-field label="Message">
                <b-input type="textarea" v-model="message" name="message"></b-input>
            </b-field>

            <div style="padding-bottom: 0.8rem;" data-netlify-recaptcha="true"></div>

            <b-button name="submitbtn" native-type="submit" type="is-danger">Envoyer</b-button>

          </form>

        </div>
      </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {

data() {
  return {
      name: null,
      email: null,
      message: null,
      errors: [],
      regexEmail: /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,24}))$/,
      regexName: /^[a-z0-9 _\-]+$/i,
      allowSubmit: false
    }
  },
  methods: {
    validateForm: function(event) {
      this.errors = [];

      let validateEmail = this.regexEmail.test(this.email);
      if (!validateEmail && (typeof(email) != undefined)) this.errors.push("Email invalide");

      if (this.errors.length <= 0) this.allowSubmit = true;
    },
  }
}

</script>

<style>

</style>
