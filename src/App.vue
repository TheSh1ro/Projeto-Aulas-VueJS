<template>
  <header id="header">
    <img src="" alt="Logo" />
    <ul class="navbar">
      <RouterLink />
      <RouterLink />
    </ul>
    <ul>
      <li>Account</li>
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
  height: 100vh;
  width: 100vw;

  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 10vh 1fr auto;
  grid-template-areas:
    "header"
    "main"
    "footer";

  font-size: 16px;
}

#header {
  grid-area: header;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;

  font-size: 1.3em;
  background-color: rgb(21, 123, 163);
}
.navbar {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  background-color: rgb(21, 123, 0);
}
.nav-item {
  color: black;
}
.nav-item:hover {
  cursor: pointer;
  background-color: rgba(0, 0, 0, 0.2);
}

#main {
  grid-area: main;
  display: flex;
  flex-direction: row;

  background-color: black;
  color: wheat;
}

#footer {
  grid-area: footer;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;

  font-size: 1.3em;
  background-color: rgb(21, 123, 163);
}
.footerbar {
  height: 100%;

  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  flex-grow: 1;
}
.footer-item {
  height: 100%;

  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  flex-grow: 1;
}
.footer-item:hover {
  cursor: pointer;
  background-color: rgba(0, 0, 0, 0.2);
}
</style>
