<template>
  <div id="app">
    <TheHeader />
    <AboutSection />
    <SocialsAndResume />
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue';
import AboutSection from '@/components/AboutSection.vue';
import SocialsAndResume from '@/components/SocialsAndResume.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    AboutSection,
    SocialsAndResume
  }
};
</script>

<style>
html, body {
  margin: 0;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-family: 'Open Sans';
  font-size: 28px;
  /* font-family: 'Roboto Slab'; */
}
h1 {
  display: block;
  font-size: 42px;
  margin: 20px 0;
  color: black;
  font-weight: normal;
}
p {
  font-size: 22px;
}
.link {
  color: rgb(0, 0, 200);
  text-decoration: underline;
  font-weight: bolder;
  cursor: pointer;
}
.minor.btn {
  padding: 14px 36px;
  border: 1px solid #707070;
  background-color: white;
  border-radius: 26px;
  text-transform: uppercase;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  font: 26px/33px "Open Sans";
  font-weight: 100;
  color: #595959;
  letter-spacing: 1.56px;
}
</style>
