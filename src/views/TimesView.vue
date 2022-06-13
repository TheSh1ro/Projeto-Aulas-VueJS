<script>
// import { v4 as uuid } from "uuid";
export default {
  data() {
    return {
      times: [
        { id: "ab0b59c9-c846-4349-904f-ba5d1cf53329", name: "Time 1" },
        { id: "1262e7a2-6ba2-405a-8ca6-044a3406afd0", name: "Time 2" },
        { id: "f5df0e90-d169-4f4f-aae3-721c03e03e59", name: "Time 3" },
        { id: "b5f66fe8-a9fc-4eb6-a26f-f690ff0512df", name: "Time 4" },
      ],
    };
  },

  methods: {
    salvar() {
      if (this.novo_time != "") {
        // const novo_id = uuid();
        this.times.push({
          id: "b5f66fe8-a9fc-4eb6-a26f-f690ff0512df",
          name: this.novo_time,
        });
        this.novo_time = "";
      }
    },
    excluir(time) {
      const indice = this.times.indexOf(time);
      this.times.splice(indice, 1);
    },
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
        <input type="text" v-model="novo_time" placeholder="Insira o time" />
        <button @click="salvar">Ok</button>
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
              <td>
                <button @click="alerta">Excluir</button>
                <button>Editar</button>
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </main>
</template>
<style scoped>
button {
  color: black;
}
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
