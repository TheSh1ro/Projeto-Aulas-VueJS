<script>
export default {
  data() {
    return {
      times: [
        { id: 1, name: "Time 1" },
        { id: 2, name: "Time 2" },
        { id: 3, name: "Time 3" },
        { id: 4, name: "Time 4" },
      ],
    };
  },
};
</script>
<template>
  <main id="main">
    <div class="form">
      <div class="form-title">
        <h1>Gerenciamento de times</h1>
      </div>
      <div class="form-input">
        <input type="text" placeholder="Insira o time" />
        <button>Ok</button>
      </div>
      <div class="form-view">
        <table>
          <thead>
            <tr>
              <th>ID</th>
              <th>Nome</th>
              <th>Ações</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="time in times" :key="time.id">
              <td>{{ time.id }}</td>
              <td>{{ time.name }}</td>
              <td>Ação</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </main>
</template>
<style scoped>
#main {
  grid-area: main;
  display: flex;
  flex-direction: column;
  align-items: stretch;
  justify-content: flex-start;
  padding: 5vh;

  background-color: black;
  color: white;
  font-size: 1em;
}
.form {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  flex-grow: 1;
}
.form-input {
  display: flex;
  align-items: stretch;
  color: black;
}
.form-input > input {
  text-align: center;
}
.form-input > button {
  padding: 5px;
}
.form-view {
  align-self: stretch;
}
table {
  width: 50%;
  border-collapse: collapse;
  margin: 0 auto;
  font-size: 1.1rem;
  text-align: center;
}
table thead {
  font-weight: bold;
  background-color: rgb(35, 35, 35);
}
table tbody tr {
  color: black;
  background-color: rgb(160, 160, 160);
}
table tbody tr:nth-child(odd) {
  color: white;
  background-color: rgb(80, 80, 80);
}
table > tbody > td,
th {
  padding: 5px;
}
</style>
