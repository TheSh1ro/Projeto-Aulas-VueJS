<script>
export default {};
</script>
<template>
  <footer id="footer">
    <nav class="footer-navbar">
      <a class="footer-navbar-item">Contato</a>
      <a class="footer-navbar-item">Telefone</a>
      <a class="footer-navbar-item">Email</a>
    </nav>
    <nav class="footer-navbar">
      <a class="footer-navbar-item">Sobre</a>
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
  justify-content: space-around;
  padding: 0.5em;

  background-color: rgb(50, 80, 160);
  font-size: 1.2em;
}
</style>
