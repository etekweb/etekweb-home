<template>
  <div class="projects section">
    <h1>Projects</h1>
    <p class="upper-p">You can take a look at some projects I’ve been involved with below.</p>
    <div class="gallery">
      <div class="gallery-item one" />
      <div class="gallery-item two" />
      <div class="gallery-item three" />
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
}
h1 {
  margin: 0;
}
.upper-p {
  margin-top: 16px;
  margin-bottom: 40px;
}
/* Default: Three items plus button inline */
.gallery {
  display: grid;
  grid-auto-flow: column;
  grid-template-columns: 320px 320px 320px 130px;
  column-gap: 32px;
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
/* Two items plus button inline */
@media screen and (max-width: 1230px) {
  .gallery {
    grid-template-columns: 320px 320px 130px;
  }
  .gallery-item.three {
    display: none;
  }
}
/* One item plus button inline */
@media screen and (max-width: 880px) {
  .gallery {
    grid-template-columns: 320px 100px;
  }
  .gallery-item.two {
    display: none;
  }
}
/* One item plus button on separate rows */
@media screen and (max-width: 500px) {
  .gallery {
    grid-template-columns: auto;
    grid-template-rows: 320px 80px;
    row-gap: 16px;
  }
  .gallery-item.two {
    display: none;
  }
}
</style>