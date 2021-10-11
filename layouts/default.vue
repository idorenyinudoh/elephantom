<template lang="pug">
  #container
    the-nav
    nuxt
</template>

<script>
import TheNav from "../components/TheNav.vue";

export default {
  components: {
    TheNav,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Overpass&display=swap');
body {
  margin: 0;
  font-family: 'Overpass', sans-serif;
  font-size: 18px;
  letter-spacing: -0.5px;
  line-height: 28px;
}
#container {
  background-color: #F5F8FF;
}
</style>