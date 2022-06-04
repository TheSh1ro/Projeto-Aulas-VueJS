<script>
export default {};
</script>
<template>
  <footer id="footer">
    <nav class="footer-navbar">
      <p class="footer-navbar-title">Contato</p>
      <a class="footer-navbar-item">Endereço</a>
      <a class="footer-navbar-item">Telefone</a>
      <a class="footer-navbar-item">Email</a>
    </nav>
    <nav class="footer-navbar">
      <p class="footer-navbar-title">Sobre</p>
      <a class="footer-navbar-item">Parceiros</a>
      <a class="footer-navbar-item">Fundação</a>
      <a class="footer-navbar-item">Projeto</a>
    </nav>
    <nav class="footer-navbar">
      <p class="footer-navbar-title">Sobre</p>
      <a class="footer-navbar-item">Parceiros</a>
      <a class="footer-navbar-item">Fundação</a>
      <a class="footer-navbar-item">Projeto</a>
    </nav>
  </footer>
</template>
<style scoped>
#footer {
  grid-area: footer;
  display: flex;
  flex-direction: row;
  align-items: stretch;
  justify-content: space-evenly;
}
.footer-navbar {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 1vh 1vw;
  cursor: default;
}
.footer-navbar-title {
  font-size: 1.2em;
  font-weight: bolder;
  border-bottom: 1px groove whitesmoke;
  margin-bottom: 5px;
}
.footer-navbar-item {
  font-size: 1em;
  cursor: pointer;
}
.footer-navbar-item:hover {
  color: rgba(255, 0, 255);
}
</style>
