<script>
export default {};
</script>
<template>
  <header id="header">
    <RouterLink to="/" class="header-logo">
      <img src="../icons/icone.png" alt="Logo" />
      <p>WebSite</p>
    </RouterLink>
    <nav class="header-navbar">
      <RouterLink to="/" class="header-navbar-item">Home</RouterLink>
      <RouterLink to="/times" class="header-navbar-item">Times</RouterLink>
      <RouterLink to="/jogadores" class="header-navbar-item">Jogadores</RouterLink>
    </nav>
  </header>
</template>
<style scoped>
#header {
  grid-area: header;
  display: flex;
  flex-direction: row;
  align-items: stretch;
  justify-content: space-around;

  border-bottom: 2px groove white;
}
.header-logo {
  display: flex;
  align-items: center;
  padding: 1vh;
  gap: 5px;
}
.header-logo > img {
  height: 30px;
}
.header-navbar {
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.header-navbar-item {
  display: flex;
  align-items: center;
  padding: 0px 40px;

  border-bottom: 2px groove white;
  margin-bottom: -2px;
}
.header-navbar-item:hover {
  background-color: rgba(0, 0, 0, 0.1);
  border-bottom: 2px groove red;
}
</style>
