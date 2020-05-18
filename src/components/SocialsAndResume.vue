<template>
  <div class="social">
    <h1>Find me on</h1>
    <img class="icon" src="@/assets/github.png">
    <img class="icon" src="@/assets/linkedin.png">
    <div class="divider" />
    <div class="minor btn">Printable Resume</div>
  </div>
</template>

<script>
export default {

};
</script>

<style scoped>
.social {
  margin: 57px 0 47px 0;
  width: 100%;
  height: 160px;
  background-color: #F0F2F2;
  display: flex;
  align-items: center;
  justify-content: center;
}
.icon {
  width: 88px;
  height: 88px;
  margin: 0 0 0 25px;
}
.divider {
  width: 1px;
  height: 75px;
  background-color: black;
  margin: 0 40px;
}
</style>