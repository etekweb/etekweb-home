<template>
  <div class="projects section">
    <h1>Projects</h1>
    <p class="upper-p">You can take a look at some projects I’ve been involved with below.</p>
    <div class="layout">
      <div class="circle-btn">&lt;</div>
      <div class="gallery">
        <div class="gallery-item one" />
        <div class="gallery-item one" />
        <div class="gallery-item one" />
        <div class="gallery-item one" />
        <div class="gallery-item one" />
        <div class="gallery-item one" />
        <div class="gallery-item one" />
        <div class="gallery-item one" />
        <div class="gallery-item one" />
        <div class="gallery-item one" />
        <div class="gallery-item one" />
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
.gallery-item {
  width: 320px;
  height: 320px;
  border: 1px solid #707070;
  border-radius: 28px;
}
.lower-p {
  margin-top: 40px;
}
</style>