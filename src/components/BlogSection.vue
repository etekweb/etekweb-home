<template>
  <div class="blog">
    <div class="post">
      ...
      <div class="minor btn">Read On</div>
    </div>
    <h1>Blog</h1>
    <div class="more-posts btn">View more posts</div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.blog {
  background-color: #F0F2F2;
  display: grid;
  justify-content: center;
  grid-template-columns: 980px 380px;
  grid-template-rows: 65px auto;
  gap: 40px;
  padding: 50px 9vw;
}
.post {
  height: 320px;
  background-color: white;
  grid-row: 1 / 3;
  border: 1px solid #707070;
  position: relative;
}
.minor.btn {
  position: absolute;
  bottom: -25px;
  left: 50%;
  transform: translateX(-50%);
}
.more-posts {
  height: 28px;
}
@media screen and (max-width: 1440px) {
  .blog {
    grid-template-columns: 1fr;
    grid-template-rows: 50px 200px 130px;
  }
  .post {
    grid-row: 2 / 3;
    height: 200px;
  }
  h1 {
    text-align: center;
  }
  .more-posts {
    width: 260px;
    margin-top: 32px;
    justify-self: center;
  }
}
@media screen and (max-width: 950px) {
  .blog {
    grid-template-rows: 50px 200px 110px;
  }
  .more-posts {
    width: 220px;
    height: unset;
  }
}
</style>