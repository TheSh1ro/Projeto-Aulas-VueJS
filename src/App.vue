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
/*Pre-sets*/

* {
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
  text-decoration: none;
  color: inherit;
  list-style-type: none;
  font-size: 1em;
}

html, body, #app {
  min-height: 100vh;
  max-width: 100%;
}

/*Scrollbar css*/

::-webkit-scrollbar {
  width: 5px;
}
::-webkit-scrollbar-thumb {
  background: rgb(55, 55, 55);
  border-radius: 0px;
  padding: 10px;
}

::-webkit-scrollbar-track {
  background: yellow;
}

/*Start*/

#app {
  font-size: 16px;
  font-family: baskerville;

  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 10vh 90vh 20vh;
  grid-template-areas:
    "header"
    "main"
    "footer";
}

#header {
  /*background-color: rgb(50, 80, 160);*/
  background-color: rgb(35, 35, 35);
  color: yellow;
  font-size: 1.3em;
}

#main {
  background-color: rgb(0, 0, 0);
  color: whitesmoke;
  font-size: 1em;
}

#footer {
  background-color: rgb(35, 35, 35);
  color: yellow;
  font-size: 1em;
}
</style>
