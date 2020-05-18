<template>
  <div id="app">
    <TheHeader />
    <AboutSection />
    <SocialsAndResume />
    <ExperienceSection />
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue';
import AboutSection from '@/components/AboutSection.vue';
import SocialsAndResume from '@/components/SocialsAndResume.vue';
import ExperienceSection from '@/components/ExperienceSection.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    AboutSection,
    SocialsAndResume,
    ExperienceSection
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
  font-size: 26px;
  line-height: 34px;
  /* font-family: 'Roboto Slab'; */
}
.section {
  margin: 0 9vw;
}
h1 {
  display: block;
  font-size: 48px;
  line-height: 65px;
  margin: 30px 0;
  color: black;
  font-weight: normal;
}
p {
  /* font-size: 22px; */
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
