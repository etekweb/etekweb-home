<template>
  <div class="experience section">
    <h1>Experience</h1>
    <p class="first">
      <b>Northland Designs</b><br>
      In this position, I worked closely with a variety of local businesses 
      to troubleshoot Windows computer system problems, 
      perform IT-related maintenance and setup tasks, 
      and train users on the use of new software and hardware.<br>
      This position also involved work with network systems, 
      including designing an office Ethernet network plan and 
      cable management in a large-office network rack.
    </p>
    <div class="second">
      <div class="left">
        <p>
          <b>24G</b><br>
          Most recently, I have been working in an internship role at 24G,
          an agency that worked with many different types of businesses
          to build high-quality digital experiences.
        </p>
        <p>
          In my role, I have been learning about the processes of web application
          development, with a primary focus on frontend.<br>
          Through this job I gained working knowledge in JavaScript and Vue.js,
          worked individually and in small teams,
          and traveled onsite with client-facing experience.
        </p>
        <p>
          My in-person internship lasted from May-December 2020,
          and I am continuing to work remotely with the company.
        </p>
      </div>
      <img class="right" src="@/assets/24g.jpg">
    </div>
  </div>
</template>

<style scoped>
h1 {
  text-align: center;
}
.second {
  margin-top: 24px;
  display: flex;
}
.second .left {
  max-width: 47vw;
}
.second .right {
  align-self: center;
  min-width: 513px;
  max-width: 36vw;
  margin-left: 32px;
}
@media screen and (max-width: 1400px) {
  .second {
    flex-direction: column;
  }
  .second .left {
    max-width: unset;
  }
  .second .right {
    max-width: 50vw;
  }
}
@media screen and (max-width: 1024px) {
  .second .right {
    min-width: unset;
    width: 100%;
    max-width: 513px;
  }
}
</style>