<template>
  <header id="header">
    <ul class="navbar">
      <li class="nav-item">Jogadores</li>
      <li class="nav-item">Times</li>
    </ul>
  </header>
  <RouterView />
  <footer id="footer">
    <ul class="footerbar">
      <li class="footer-item">Sobre</li>
    </ul>
  </footer>
</template>
<style>
* {
  list-style-type: none;
  padding: 0px;
  margin: 0px;
}
#app {
  font-size: 16px;
  height: 100vh;
  width: 100vw;

  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 10vh auto 8vh;
  grid-template-areas:
    "header"
    "content"
    "footer";
}

#header {
  grid-area: "header";
  display: flex;
  flex-direction: row;
  align-items: center;

  font-size: 1.3em;
  background-color: darkred;
}
.navbar {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  flex-grow: 1;
  height: 100%;
}
.nav-item {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  flex-grow: 1;
  height: 100%;
}
.nav-item:hover {
  cursor: pointer;
  background-color: rgba(0, 0, 0, 0.2);
}

#content {
  grid-area: "content";
  display: flex;
  flex-direction: row;

  background-color: black;
  color: wheat;
}

#footer {
  grid-area: "footer";
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;

  font-size: 1.3em;
  background-color: darkred;
}
.footerbar {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  flex-grow: 1;
  height: 100%;
}
.footer-item {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  flex-grow: 1;
  height: 100%;
}
.footer-item:hover {
  cursor: pointer;
  background-color: rgba(0, 0, 0, 0.2);
}
</style>
