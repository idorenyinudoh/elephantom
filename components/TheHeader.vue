<template lang="pug">
h1 Acumen Digital Interview Task / Elephantom
  span(v-if="extra") &nbsp;&nbsp;&nbsp; > &nbsp;&nbsp;&nbsp; {{ extra }}
</template>

<script>
export default {
  props: {
    extra: {
      type: String,
      required: false,
      default: "",
    },
  }
};
</script>

<style scoped>
h1 {
  margin: 0;
  height: max-content;

  /* box-shadow: 0 -7px 24px rgba(0, 0, 0, 0.25); */

  /* improvised because the actual box shadow was affecting the color of the nav */

  box-shadow: 1px 3px 3px rgba(0, 0, 0, 0.25);
  padding: 25px;
  font-weight: 400;
  font-size: 18px;
  background-color: #FFF;
}
</style>