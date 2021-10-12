<template lang="pug">
nav
  #image-container
    img(src="elephant.png" alt="elephant image")
  nuxt-link(to="/") Home
  nuxt-link(to="/elephant") Elephant
</template>

<style scoped>
@media screen and (max-width: 1023px) {
  nav {
    padding-left: calc(15px + 1vw);
    grid-template-columns: repeat(3, max-content);
    column-gap: 20px;
    align-items: center;
  }
  #image-container {
    width: calc(70px + 2vw);
    margin: calc(10px + 1vw) 0;
    padding-top: 100%;
  }
  a {
    padding: calc(31px + 2vw) calc(10px + 1vw);
  }
}
@media screen and (min-width: 1024px) {
  nav {
    grid-template-rows: repeat(3, max-content);
    width: calc(250px + 1vw);
    height: 100vh;
  }
  #image-container {
    width: calc(150px + 1vw);
    margin: calc(50px + 1vw) 50px;
    padding-top: calc(100% - 100px);
  }
  a {
    padding: 15px 30px;
    align-self: baseline;
  }
}
nav {
  display: grid;
  background-color: #DDF;
}
#image-container {
  position: relative;
  background-color: #FFF;
  border-radius: 50%;
}
img {
  position: absolute;
  width: 67%;
  top: 19%;
  left: 16.5%;
}
a {
  text-decoration: none;
  color: #000;
}
.nuxt-link-exact-active {
  background-color: #B9B9FF;
  color: #FFF;
}
</style>