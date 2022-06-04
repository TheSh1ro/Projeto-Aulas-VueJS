<script setup>
import PageHeader from "./components/templates/PageHeader.vue";
import PageFooter from "./components/templates/PageFooter.vue";
</script>
<template>
  <PageHeader />
  <RouterView />
  <PageFooter />
</template>
<style>
* {
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
  text-decoration: none;
  color: inherit;
  list-style-type: none;
}
#app {
  font-size: 16px;
  height: 100vh;
  width: 100vw;

  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 8vh auto 8vh;
  grid-template-areas:
    "header"
    "main"
    "footer";
}
</style>
