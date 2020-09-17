<template>
  <div class="projects section">
    <h1>Projects</h1>
    <p class="upper-p">You can take a look at some projects I’ve been involved with below.</p>
    <div class="layout">
      <div class="circle-btn">&lt;</div>
      <div class="gallery">
        <ProjectItem v-for="(project, index) of projects" :project="project" :key="index" />
      </div>
      <div class="circle-btn">&gt;</div>
    </div>
    <p class="lower-p">
      I am always interested in new concepts and building new skills.<br>
      Have an idea? <span class="link">Let’s talk</span>.
    </p>
  </div>
</template>

<script>
import ProjectItem from "@/components/ProjectItem.vue";

export default {
  components: {
    ProjectItem,
  },
  data() {
    return {
      projects: [
        {
          name: "Salesforce #Dreamforce",
          img: "salesforce.png",
          desc: "Built an interactive display for Salesforce's Customer360 platform, as well as an interactive vending experience for ConAgra and Google Cloud.",
          languages: ["Vue.js", "HTML/CSS", "Onsite"],
        },
        {
          name: "GM Virtual Solutions Summit",
          img: "vss.png",
          desc: "Built a heavily customized event site for GM fleet customers and suppliers.",
          languages: ["Vue.js", "API Integration", "HTML/CSS"],
        },
        {
          name: "HuskyHunt",
          img: "hh.png",
          desc: "Built a site for Michigan Tech students to sell used goods, as well as find rideshares, in the campus community.",
          languages: ["MTU", "Team Lead", "Django"],
        },
        {
          name: "OnStar Vehicle Insights Demo",
          img: "ovi.png",
          desc: "Built an offline-ready site to demonstrate OnStar's fleet management capabilities for GM trade shows.",
          languages: ["Vue.js", "HTML/CSS"],
        },
        {
          name: "ABB Idea Wall",
          img: "abb.png",
          desc: "Built a site for industry professionals to view and share ideas for reducing energy consumption.",
          languages: ["Vue.js", "HTML/CSS"],
        },
      ],
    };
  },
}
</script>

<style scoped>
.projects {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
h1 {
  margin: 0;
}
.upper-p {
  margin-top: 16px;
  margin-bottom: 40px;
}
/* Default: Three items plus button inline */
.layout {
  display: grid;
  grid-auto-flow: column;
  grid-template-columns: 70px 1fr 70px;
  column-gap: 32px;
  align-items: center;
  justify-items: center;
}
.gallery {
  display: grid;
  width: 100%;
  grid-auto-flow: column;
  column-gap: 32px;
  overflow: scroll;
  align-items: center;
  justify-items: center;
}
.lower-p {
  margin-top: 40px;
}
</style>