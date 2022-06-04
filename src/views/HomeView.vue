<template>
  <main id="main">
    <section class="block">Página inicial</section>
  </main>
</template>
<style scoped>
#main {
  grid-area: main;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  padding: 5vh;

  background-color: black;
  color: white;
  font-size: 1em;
}
.block {
  padding: 1vh;
  border: purple 6px groove;
}
</style>
