<template>
  <div id="app">
    <TheHeader />
    <AboutSection />
    <SocialsAndResume />
    <ExperienceSection />
    <ProjectsSection />
    <InterestsSection />
    <ContactSection />
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue';
import AboutSection from '@/components/AboutSection.vue';
import SocialsAndResume from '@/components/SocialsAndResume.vue';
import ExperienceSection from '@/components/ExperienceSection.vue';
import ProjectsSection from '@/components/ProjectsSection.vue';
import InterestsSection from '@/components/InterestsSection.vue';
import ContactSection from '@/components/ContactSection.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    AboutSection,
    SocialsAndResume,
    ExperienceSection,
    ProjectsSection,
    InterestsSection,
    ContactSection
  }
};
</script>

<style>
html, body {
  margin: 0;
}
/* br {
  content: " ";
  display: block;
  margin: 0.34em;
} */
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-family: 'Open Sans';
  font-size: 1.3em;
  line-height: 1.5em;
}
.section {
  margin: 50px 9vw;
}
h1 {
  display: block;
  font-size: 1.75em;
  line-height: 1.25em;
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
.btn {
  padding: 34px 60px;
  border: 1px solid #707070;
  background-color: white;
  border-radius: 20px;
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
.minor.btn {
  padding: 8px 36px;
  font-size: 23px;
}
.circle-btn {
  width: 60px;
  height: 60px;
  background-color: white;
  border: 1px solid #707070;
  border-radius: 50%;
  text-align: center;
  font: 30px/40px 'Open Sans';
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
  .btn {
    font-size: 21px;
    line-height: 31px;
  }
  .minor.btn {
    font-size: 18px;
    line-height: 28px;
  }
  .circle-btn {
    width: 40px;
    height: 40px;
    font-size: 18px;
    line-height: 22px;
  }
}
b {
  margin: 8px 0;
  display: inline-block;
}
</style>
