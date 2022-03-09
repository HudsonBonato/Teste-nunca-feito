<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />

    <h1>Lista de Usuarios</h1>

    <div class="container" id="lista-home">
      <ul class="list-group list-group-numbered">
        <li v-for="(list, key) in data" class="list-group-item" :key="key">
          {{ list.nome }} - {{ list.sobrenome }} - {{ list.celular }} -
          {{ list.endereco }}
        </li>
      </ul>
    </div>
  </div>
</template>


<script>
// @ is an alias to /src

export default {
  name: "Home",
  data() {
    return {
      data: [],
      nome: "",
      sobrenome: "",
      celular: "",
      endereco: "",
    };
  },
  methods: {
    salvar() {
      this.axios
        .post("http://127.0.0.1:8000/teste", {
          nome: this.nome,
          sobrenome: this.sobrenome,
          celular: this.celular,
          endereco: this.endereco,
        })
        .then((response) => {
          console.log(response.data);
          this.sobrenome = response.data.sobrenome;
          this.celular = response.data.celular;
          this.endereco = response.data.endereco;
        });
    },
  },
  mounted() {
    this.axios.get("http://127.0.0.1:8000/teste-view").then((response) => {
        this.data = response.data;
      });
  }
};
</script>

<style scoped>

h1 {
    background-color: #41b883;
    margin-left: 300px;
    margin-right: 300px;
    margin-bottom: 20px;
    font-size: 50px;
    color: #FFF;
}
</style>

