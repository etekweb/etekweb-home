<template>
  <div class="header">
    Ethan Matzdorf
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.header {
  width: 100%;
  min-height: 400px;
  max-height: 50vh;
  background-image: url('../assets/banner.jpg');
  background-position-y: bottom;
  background-size: 100vw;
  background-repeat: no-repeat;
  background-size: cover;
  background-position-x: center;
  display: flex;
  align-items: center;
  justify-content: center;
  font: 70px/96px 'Open Sans';
  letter-spacing: 0px;
  color: #FFFFFF;
  text-align: center;
  text-shadow:
		-1px -1px 0 #707070,
		1px -1px 0 #707070,
		-1px 1px 0 #707070,
		1px 1px 0 #707070;
}
</style>