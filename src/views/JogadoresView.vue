<template>
  <main id="main">
    <div class="cadastro">
      <h1>Cadastrar jogadores</h1>
      <section>
        <span>Nome</span>
        <input type="text" />
      </section>
      <section>
        <span>Idade</span>
        <input type="text" />
      </section>
    </div>
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
.cadastro {
  display: flex;
  flex-direction: column;
}
</style>
