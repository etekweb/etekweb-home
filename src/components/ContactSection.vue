<template>
  <div class="contact-section">
    <CalendarModal v-if="showCalModal" @done="showCalModal = false" />
    <h1>Contact Me</h1>
    <form class="contact-details" action="https://formsubmit.co/1f76f55e81e934d2f67b6ca613097ba2" method="POST">
      <div class="contact-fields">
        <span>Your Name</span>
        <input v-model="name" />
        <span>Your Email</span>
        <input v-model="email" type="email" name="email" />
        <span>Subject</span>
        <input v-model="subject" name="_subject" />
        <span class="message-lbl">Message</span>
        <textarea rows="8" v-model="message" name="message" />
      </div>
      <div class="final-section">
        <!-- <vue-recaptcha
          class="recaptcha"
          sitekey="6LfCCLUUAAAAADRkxjo3gHcVXlZGouubHmdEpxYa"
          :loadRecaptchaScript="true"
          @verify="handleCaptcha"
          @expired="unhandleCaptcha"
        /> -->
        <!-- @click="submit" -->
        <button class="btn" type="submit">Send Message</button>
      </div>
    </form>
    <span class="msg">
      Looking to schedule a meeting?
      <span class="link" @click="showCalModal = true">Click here</span> to see my free/busy calendar.
    </span>
  </div>
</template>

<script>
// import VueRecaptcha from "vue-recaptcha";
import Axios from "axios";

import CalendarModal from "@/components/CalendarModal.vue";

export default {
  data() {
    return {
      // Fields are modeled for future contact form usage
      name: "",
      email: "",
      subject: "",
      message: "",
      captcha: "",
      // Variable to show/hide the web calendar (link at bottom)
      showCalModal: false,
    };
  },
  components: {
    // VueRecaptcha,
    CalendarModal,
  },
  computed: {
    readyToSubmit() {
      if (
        this.name &&
        this.email &&
        this.subject &&
        this.message &&
        this.captcha
      ) {
        return true;
      }
      return false;
    },
  },
  methods: {
    handleCaptcha(data) {
      this.captcha = data;
    },
    unhandleCaptcha() {
      this.captcha = "";
    },
    submit() {
      if (this.readyToSubmit) {
        Axios.post(
          "https://us-central1-etekweb-7bb7d.cloudfunctions.net/sendMail",
          {
            name: this.name,
            email: this.email,
            subject: this.subject,
            message: this.message,
            "g-recaptcha-response": this.captcha,
          }
        )
          .then(() => {
            console.log("good");
            alert("Your message was sent successfully!");
          })
          .catch((err) => {
            console.dir(err);
            alert(
              "Something went wrong when sending your message. Please try again."
            );
          });
      } else {
        alert("Please ensure all fields are filled before submitting!");
      }
    },
  },
};
</script>

<style scoped>
.contact-section {
  background-color: #f0f2f2;
  padding: 60px 10vw 100px 10vw;
}
.contact-details {
  display: flex;
}
.contact-fields {
  display: grid;
  grid-template-rows: 50px 50px 50px 150px;
  grid-template-columns: 120px 500px;
  gap: 16px;
  align-items: center;
}
.contact-fields span {
  justify-self: right;
}
input, textarea {
  border: 1px solid black;
  font-family: 'Open Sans';
  border-radius: 3px;
}
input {
  height: 30px;
}
textarea {
  max-height: 130px;
}
.final-section {
  margin-left: 40px;
}
.message-lbl {
  align-self: start;
  margin-top: 16px;
}
@media screen and (max-width: 1234px) {
  .contact-details {
    display: unset;
  }
}
.btn {
  padding: 14px 40px;
  font-size: unset;
  margin-top: 6px;
  margin-left: auto;
}
.msg {
  font-size: 16px;
}
.msg .link {
  text-decoration: underline;
  color: blue;
  cursor: pointer;
}
</style>