<template>
  <div class="about section">
    <div class="about-text">
      <h1>Hello, world!</h1>
      <p>
        My name is Ethan Matzdorf. 
        I was born and raised in Cloquet, MN and am currently pursuing a B.S. in Computer Science from 
        Michigan Technological University.
      </p>
      <p>
        From a young age, I have taken great interest in technology in various forms, exploring and 
        learning about all of the many possibilities they contain.<br>
        I experimented with rudimentary web design starting at age seven, 
        and in sixth grade began learning the basics of HTML, CSS, PHP and MySQL.<br>
        From there, I took initiative in developing web projects for my community 
        that are in production use today: a registration utility for a middle school enrichment class program, 
        and a trail map system at a local park.
      </p>
      <p>
        In college, I have been working for 24G, a digital experience agency, as a JavaScript developer.
        <!-- TODO - add link to section when added -->
        <span class="link">See what I did there</span>.
      </p>
    </div>
    <img class="profile-img" src="@/assets/profile.jpg">
  </div>
</template>

<style scoped>
.about {
  margin-top: 55px;
  display: flex;
}
.about-text {
  max-width: 57vw;
  margin-right: 4vw;
}
.profile-img {
  width: 22vw;
  align-self: center;
}
@media screen and (max-width: 1114px) {
  .about {
    flex-direction: column;
  }
  .about-text {
    max-width: unset;
  }
  .profile-img {
    width: 34vw;
  }
}
</style>