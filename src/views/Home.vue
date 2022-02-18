<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />

    <h1>Lista de Usuarios</h1>

    <form>
      <div class="container" id="login-home">
        <div class="mb-3">
          <label for="exampleInputEmail1" class="form-label"
            >Endereço de email</label
          >
          <input
            type="email"
            class="form-control"
            id="exampleInputEmail1"
            aria-describedby="emailHelp"
          />
          <div id="emailHelp" class="form-text">
            Nunca compartilharemos seu e-mail com mais ninguém.
          </div>
        </div>
        <div class="mb-3">
          <label for="exampleInputPassword1" class="form-label">Senha</label>
          <input
            type="password"
            class="form-control"
            id="exampleInputPassword1"
          />
        </div>
        <div class="mb-3 form-check">
          <input type="checkbox" class="form-check-input" id="exampleCheck1" />
          <label class="form-check-label" for="exampleCheck1"
            >Lembre de mim</label
          >
        </div>
        <button type="submit" class="btn btn-primary">Enviar</button>
      </div>
    </form>

    <div class="container" id="lista-home">
      <ol class="list-group list-group-numbered">
        <li class="list-group-item">Usuario</li>
      </ol>
    </div>
  </div>
</template>


<script>
// @ is an alias to /src

export default {
  name: "Home",
};
</script>

<!--<style scoped>
h1 {
    background-color: #354;
    font-size: 50px;
    color: #FFF
}
</style>-->

