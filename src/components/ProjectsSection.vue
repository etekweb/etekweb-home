<template>
  <div class="projects">
    <h1>Projects</h1>
    <p class="upper-p">You can take a look at some projects I’ve been involved with below.</p>
    <div class="gallery">
      <div class="gallery-item" />
      <div class="gallery-item" />
      <div class="gallery-item" />
      <div class="circle-btn">View more</div>
    </div>
    <p class="lower-p">
      I am always interested in new concepts and building new skills.<br>
      Have an idea? <span class="link">Let’s talk</span>.
    </p>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.projects {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin: 67px 0;
}
h1 {
  margin: 0;
}
.upper-p {
  margin-top: 16px;
  margin-bottom: 40px;
}
.gallery {
  display: grid;
  grid-auto-flow: column;
  grid-template-columns: 360px 360px 360px 177px;
  column-gap: 32px;
  align-items: center;
  justify-items: center;
}
.gallery-item {
  width: 360px;
  height: 360px;
  border: 1px solid #707070;
  border-radius: 28px;
}
.lower-p {
  margin-top: 40px;
}
</style>