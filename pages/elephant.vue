<template lang="pug">
#elephant-container
  the-header(extra="Elephant")
  main
    #image-container
      img(src="tuffi.png" alt="an image of a tuffi looking heart-broken")
    h2 Tuffi
    p Female
    hr
    p A female circus elephant that became famous in Germany during 1950 when she accidentally fell into the River Wupper, and survived.
</template>

<script>
import TheHeader from "../components/TheHeader.vue";

export default {
  components: {
    TheHeader,
  },
};
</script>

<style scoped>
#elephant-container {
  color: #30425A;
}
main {
  padding: 40px;
}
#image-container {
  position: relative;
  padding-top: 45.6%;
}
#image-container::after {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  content: '';
  background: linear-gradient(180deg, rgba(196, 196, 196, 0) -1.55%, rgba(29, 29, 242, 0.37) 77.84%);
}
img {
  position: absolute;
  width: 100%;
  top: 0;
  left: 0;
}
h2 {
  display: inline-block;
  margin: 40px 0;
  width: max-content;
  font-size: 48px;
  line-height: 74px;
}
p {
  margin: calc(20px + 1vw) 0;
}
p:first-of-type {
  display: inline-block;
  margin-left: calc(16px + 1vw);
}
hr {
  width: 100%;
  height: 1px;
  margin: 0;
  border: 0;
  background-color: #C4CDD59E;
}
</style>