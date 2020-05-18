<template>
  <div class="social">
    <h1>Find me on</h1>
    <img class="icon" @click="goToGithub" src="@/assets/github.png">
    <img class="icon" @click="goToLinkedin" src="@/assets/linkedin.png">
    <div class="divider" />
    <div class="minor btn" @click="goToResume">Printable Resume</div>
  </div>
</template>

<script>
export default {
  methods: {
    goToGithub() {
      window.open('https://github.com/etekweb', '_blank');
    },
    goToLinkedin() {
      window.open('https://www.linkedin.com/in/ethan-matzdorf-9493b4137/', '_blank');
    },
    goToResume() {
      // TODO - Add link to page when added
    }
  }
};
</script>

<style scoped>
.social {
  margin: 57px 0 47px 0;
  width: 100%;
  height: 160px;
  background-color: #F0F2F2;
  display: flex;
  align-items: center;
  justify-content: center;
}
.icon {
  width: 88px;
  height: 88px;
  border-radius: 50%;
  margin: 0 0 0 25px;
  cursor: pointer;
}
.divider {
  width: 1px;
  height: 75px;
  background-color: black;
  margin: 0 40px;
}
</style>