<script>
export default {};
</script>
<template>
  <header id="header">
    <div class="navbar">
      <RouterLink to="/times" class="nav-item">Times</RouterLink>
      <RouterLink to="/" class="nav-item">Home</RouterLink>
      <RouterLink to="/jogadores" class="nav-item">Jogadores</RouterLink>
    </div>
  </header>
</template>
<style scoped>
#header {
  grid-area: header;
  display: flex;
  flex-direction: row;
  align-items: stretch;
  justify-content: center;

  background-color: rgb(50, 80, 160);
  font-size: 1.3em;
}
.navbar {
  display: flex;
  flex-direction: row;
  align-items: stretch;
  justify-content: space-evenly;
  flex-grow: 1;
}
.nav-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  flex-grow: 1;

  border-bottom: 2px ridge black;

  cursor: pointer;
  text-decoration: none;
  color: inherit;
}
.nav-item:nth-child(2) {
  border-inline: 2px solid black;
}
.nav-item:hover {
  background-color: rgb(0, 0, 0, 0.1);
  border-bottom: 2px ridge darkred;
}
</style>
