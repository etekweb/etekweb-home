<template>
  <div id="app">
    <TheHeader />
    <div class="about">
      <h1>Hello, world!</h1>
      <p>
        My name is Ethan Matzdorf. 
        I was born and raised in Cloquet, MN and am currently pursuing a B.S. in Computer Science from Michigan Technological University.
      </p>
      <p>
        From a young age, I have taken great interest in technology in various forms, exploring and learning about all of the many possibilities they contain.<br>
        I experimented with rudimentary web design starting at age seven, and in sixth grade began learning the basics of HTML, CSS, PHP and MySQL.<br>
        From there, I took initiative in developing web projects for my community that are in production use today: a registration utility for a middle school enrichment class program, and a trail map system at a local park.
      </p>
      <p>
        In college, I have been working for 24G, a digital experience agency, as a JavaScript developer.<br>
        <!-- TODO - add link to section when added -->
        <span class="link">See what I did there</span>.
      </p>
    </div>
    <SocialsAndResume />
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue';
import SocialsAndResume from '@/components/SocialsAndResume.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
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
.about {
  margin-top: 55px;
  margin-left: 9vw;
  max-width: 57vw;
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
