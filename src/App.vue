<template>
  <div id="app">
    <TheHeader />
    <AboutSection />
    <SocialsAndResume />
    <ExperienceSection />
    <ProjectsSection />
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue';
import AboutSection from '@/components/AboutSection.vue';
import SocialsAndResume from '@/components/SocialsAndResume.vue';
import ExperienceSection from '@/components/ExperienceSection.vue';
import ProjectsSection from '@/components/ProjectsSection.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    AboutSection,
    SocialsAndResume,
    ExperienceSection,
    ProjectsSection
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
  font-size: 1.3em;
  line-height: 1.5em;
}
.section {
  margin: 0 9vw;
}
h1 {
  display: block;
  font-size: 1.75em;
  line-height: 2em;
  margin: 16px 0;
  color: black;
  font-weight: normal;
}
.link {
  color: rgb(0, 0, 200);
  text-decoration: underline;
  font-weight: bolder;
  cursor: pointer;
}
.minor.btn {
  padding: 8px 36px;
  border: 1px solid #707070;
  background-color: white;
  border-radius: 20px;
  text-transform: uppercase;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  font: 23px/33px "Open Sans";
  font-weight: 100;
  color: #595959;
  letter-spacing: 1.56px;
}
.circle-btn {
  width: 100px;
  height: 100px;
  background-color: white;
  border: 1px solid #707070;
  border-radius: 50%;
  text-align: center;
  font: 22px/28px 'Open Sans';
  font-weight: 100;
  letter-spacing: 1.56px;
  color: #595959;
  text-transform: uppercase;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}
/* Lower font sizes on smaller screens */
@media screen and (max-width: 950px) {
  #app {
    font-size: 1.1em;
    line-height: 1.3em;
  }
  .minor.btn {
    font-size: 18px;
    line-height: 28px;
  }
  .circle-btn {
    width: 80px;
    height: 80px;
    font-size: 18px;
    line-height: 22px;
  }
}
</style>
