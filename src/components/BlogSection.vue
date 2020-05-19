<template>
  <div class="blog">
    <div class="post">

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
  grid-template-columns: 1000px 380px;
  grid-template-rows: 65px auto;
  gap: 40px 67px;
  padding: 50px 9vw;
}
.post {
  width: 980px;
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
</style>