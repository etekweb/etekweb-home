<template>
  <div id="app">
    <TheHeader />
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
  }
};
</script>

<style>
html, body {
  margin: 0;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-family: 'Open Sans';
  /* font-family: 'Roboto Slab'; */
}
</style>
