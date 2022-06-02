<template>
  <header id="header">
    <div class="navbar">
      <span class="nav-item">Teams</span>
      <span class="nav-item">Players</span>
    </div>
  </header>
  <RouterView />
  <footer id="footer">
    <div class="footer-social">
      <span class="social-item">Instagram</span>
      <span class="social-item">Twitter</span>
    </div>
    <div class="footer-social">
      <span class="social-item">Instagram</span>
      <span class="social-item">Twitter</span>
    </div>
    <div class="footer-social">
      <span class="social-item">Instagram</span>
      <span class="social-item">Twitter</span>
    </div>
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
  grid-template-rows: 7vh auto 8vh;
  grid-template-areas:
    "header"
    "main"
    "footer";
}

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
  flex-direction: row;
  align-items: center;
  justify-content: center;
  flex-grow: 1;

  border-bottom: 2px ridge black;
  cursor: pointer;
}
.nav-item:hover {
  background-color: rgb(0, 0, 0, 0.1);
  border-bottom: 2px ridge darkred;
}
#main {
  grid-area: main;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  background-color: black;
  color: white;
  font-size: 1em;
}
.block {
  padding: 1vh;
  border: purple 5px groove;
}
#footer {
  grid-area: footer;
  display: flex;
  flex-direction: row;
  align-items: stretch;
  justify-content: space-evenly;
  padding: 5px;

  background-color: rgb(50, 80, 160);
  font-size: 0.95em;
}
.footer-social {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-evenly;
}
.social-item {
  cursor: pointer;
}
.social-item:hover {
  color: rgb(30, 30, 30);
}
</style>
