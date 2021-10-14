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
      footer
        p PAGE 1 OF 10
        button.icon(disabled) <
        button.active 1
        button 2
        button.icon >
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
  position: absolute;
  top: 0;
  width: calc(100% - 56px);
  padding: 26px;
  font-size: 18px;
  font-weight: bold;
  line-height: 28px;
  color: #30425A;
  background-color: #FFF;
  text-align: left;
}
table {
  position: relative;
  padding-top: 80px;
  width: 100%;
  box-shadow: 0 3px 10px -3px rgba(0, 0, 0, 0.25);
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
footer {
  margin: 0;
  padding: 40px;
  display: grid;
  grid-template-columns: repeat(5, max-content);
  column-gap: 10px;
  justify-content: center;
  align-items: center;
  font-size: 14px;
  background-color: #FFF;
}
footer p {
  margin: 0;
}
button {
  background: inherit;
  border: 1px solid #DFE3E8;
  border-radius: 20%;
  padding: 0;
  width: 32px;
  height: 32px;
  color: #000;
}
button:disabled {
  background-color: #919EAB;
  opacity: 0.5;
}
button:not(:disabled) {
  cursor: pointer;
}
.active, button:not(:disabled):hover {
  border-color: #0546E0;
  color: #0546E0;
}
.icon {
  color: #C4CDD5;
}
</style>
