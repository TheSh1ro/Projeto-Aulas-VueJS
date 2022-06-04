<template>
  <main id="main">
    <img class="home-image" src="https://i.ytimg.com/vi/yFOdkyaoUTg/hqdefault.jpg?sqp=-oaymwEbCKgBEF5IVfKriqkDDggBFQAAiEIYAXABwAEG&rs=AOn4CLDsYakMSnJ7MduNMOJseBUEA0olDQ">
    <section class="home-about">
      <div class="main-introduction">
        <h1 class="container-title">Quem somos
        </h1>
        <p class="introduction-text">Para facilitar a interação e possibilitar a contratação de jogadores, ou mesmo a criação de times, sentimos a necessidade de surgir no mercado
        </p>
      </div>
    
      <div class="main-description">
        <h1 class="container-title">
        O que posso fazer?
        </h1>
        <ul class="description-advantages">
          <h2>Caso você seja dono de um time, ou queira iniciar seu projeto</h2>
          <li>Crie seu time</li>
          <li>Gerencie seu time</li>
          <li>Encontre novos jogadores</li>
        </ul>
        <hr>
        <ul class="description-advantages">
          <h2>Caso você seja um atleta</h2>
          <li>Ingresse em um time</li>
          <li>Conheça os times</li>
          <li>Se coloque a disposição para participar de outros times como Free Agent</li>
        </ul>
      </div>
    </section>
    
  </main>
</template>
<style scoped>

#main {
  grid-area: main;
  display: flex;
  flex-direction: column;
  align-items: stretch;
  justify-content: flex-start;
}

.home-image {
  height: 20vh;
}
.home-about {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
}

.main-introduction {
  display: flex;
  flex-direction: column;
  align-items: center;
  flex-grow: 1;
}
.introduction-text {
  display: flex;
  align-items: center;
  flex-grow: 1;
}

.main-description {
  display: flex;
  flex-direction: column;
  align-items: center;
  flex-grow: 1;
}
.main-description > hr {
  align-self: center;
  width: 5%;
}
.description-advantages {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  flex-grow: 1;
}
.description-advantages > h2 {
  border-bottom: 1px groove yellow;
  margin: 5px;
  padding-inline: 1em;
}

.container-title {
  align-self: stretch;
  padding: 1em;
  text-align: center;  
  color: black;
  background: rgb(200,200,0);
}

</style>
