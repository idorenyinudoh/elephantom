<template lang="pug">
div
  the-header
  main
    table
      caption All Elephants
      thead
        tr
          th S/N
          th Name
          th Species
          th Sex
          th Affiliation
          th DoB
      tbody
        tr
          td 1
          td Name
          td Species
          td Sex
          td Affiliation
          td DoB
        tr
          td 2
          td Name
          td Species
          td Sex
          td Affiliation
          td DoB
        tr
          td 3
          td Name
          td Species
          td Sex
          td Affiliation
          td DoB
        tr
          td 4
          td Name
          td Species
          td Sex
          td Affiliation
          td DoB
        tr
          td 5
          td Name
          td Species
          td Sex
          td Affiliation
          td DoB
        tr
          td 6
          td Name
          td Species
          td Sex
          td Affiliation
          td DoB
        tr
          td 7
          td Name
          td Species
          td Sex
          td Affiliation
          td DoB
        tr
          td 8
          td Name
          td Species
          td Sex
          td Affiliation
          td DoB
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
main {
  padding: 40px;
  overflow-x: auto;
}
caption {
  margin: 0;
  padding: 26px;
  font-size: 18px;
  font-weight: bold;
  line-height: 28px;
  color: #30425A;
  background-color: #FFF;
  text-align: left;
}
table {
  width: 100%;
}
th, td {
  padding: 0;
}
tr {
  display: grid;
  padding: 26px;
  grid-template-columns: 31px 46px 59px 28px 74px 33px;
  column-gap: 20px;
  justify-content: space-between;
  text-align: center;
}
tr:nth-child(even) {
  background-color:#F5F5F5;
}
tr:nth-child(odd) {
  background-color:#FFF;
}
thead tr:first-of-type {
  background-color: #E5E5E5 !important;
}
</style>
