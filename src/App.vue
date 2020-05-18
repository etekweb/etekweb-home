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
  font-size: 23px;
  line-height: 33px;
}
.section {
  margin: 0 9vw;
}
h1 {
  display: block;
  font-size: 42px;
  line-height: 54px;
  margin: 30px 0;
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
  padding: 14px 36px;
  border: 1px solid #707070;
  background-color: white;
  border-radius: 26px;
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
  width: 129px;
  height: 129px;
  background-color: white;
  border: 1px solid #707070;
  border-radius: 50%;
  text-align: center;
  font: 26px/33px 'Open Sans';
  font-weight: 100;
  letter-spacing: 1.56px;
  color: #595959;
  text-transform: uppercase;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
