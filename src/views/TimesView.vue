<template>
  <main id="main">
    <div class="cadastro">
      <h1>Cadastrar time</h1>
      <section class="form-block">
        <input type="text" />
        <span>Nome do time</span>
      </section>
      <section class="form-block">
        <input type="text" />
        <span>País de origem</span>
      </section>
      <section class="form-block">
        <input type="text" />
        <span>Cidade de origem</span>
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
  justify-content: space-evenly;
}
.form-block {
  display: flex;
  flex-direction: row;

  background-color: rgba(0, 255, 255, 0.281);
}
</style>
