<template>
  <div class="gallery-item">
    <img class="item-bg" :src="project.img ? require('@/assets/' + project.img) : ''" />
    <div class="text-overlay">
      <div class="title">{{project.name}}</div>
      <div class="desc">{{project.desc}}</div>
      <div class="langs">
        <div class="lang" v-for="(language, index) of project.languages" :key="index">{{language}}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    project: Object,
  }
}
</script>

<style scoped>
.gallery-item {
  width: 320px;
  height: 320px;
  border: 1px solid #707070;
  border-radius: 28px;
  position: relative;
  background-color: black;
}
.item-bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  opacity: 0.4;
  border-radius: 28px;
}
.text-overlay {
  padding: 16px;
  box-sizing: border-box;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  color: white;
  display: grid;
  grid-template-rows: 80px 135px 30px;
  font-size: 18px;
  line-height: 25px;
  gap: 12px;
  align-items: center;
  justify-items: center;
  text-align: center;
}
.title {
  font-size: 27px;
  line-height: 40px;
}
.langs {
  display: grid;
  grid-auto-flow: column;
  gap: 8px;
}
.lang {
  padding: 0px 8px;
  border: 1px solid white;
  border-radius: 12px;
  font-size: 14px;
}
</style>