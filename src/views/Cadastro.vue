<template>
  <div>
    <h1>Cadastro de Usuarios</h1>

    <!-- https://bbbootstrap.com/snippets/bootstrap-5-myprofile-90806631 -->

    <div class="container rounded bg-white mt-5 mb-5">
      <div class="row">
        <div class="col-md-3 border-right">
          <div
            class="d-flex flex-column align-items-center text-center p-3 py-5"
          >
            <img
              class="rounded-circle mt-5"
              width="150px"
              src="https://st3.depositphotos.com/15648834/17930/v/600/depositphotos_179308454-stock-illustration-unknown-person-silhouette-glasses-profile.jpg"
            /><span class="font-weight-bold">Usuario</span
            ><span class="text-black-50">usuario@mail.com</span>Masculino
            <span></span>
          </div>
        </div>
        <div class="col-md-5 border-right">
          <div class="p-3 py-5">
            <div class="d-flex justify-content-between align-items-center mb-3">
              <h4 class="text-right">Configurações de Perfil</h4>
            </div>
            <div class="row mt-2">
              <div class="col-md-6">
                <label class="labels">Nome</label
                ><input
                  type="text"
                  class="form-control"
                  placeholder="Primeiro Nome"
                  value=""
                />
              </div>
              <div class="col-md-6">
                <label class="labels">Sobrenome</label
                ><input
                  type="text"
                  class="form-control"
                  value=""
                  placeholder="Sobrenome"
                />
              </div>
            </div>
            <div class="row mt-3">
              <div class="col-md-12">
                <label class="labels">Celular</label
                ><input
                  type="text"
                  class="form-control"
                  placeholder="Digite o numero do Celular"
                  value=""
                />
              </div>
              <div class="col-md-12">
                <label class="labels">Endereço</label
                ><input
                  type="text"
                  class="form-control"
                  placeholder="Digite o endereço"
                  value=""
                />
              </div>
              <div class="col-md-12">
                <label class="labels">Bairro</label
                ><input
                  type="text"
                  class="form-control"
                  placeholder="Digite o Bairro"
                  value=""
                />
              </div>
              <div class="col-md-12">
                <label class="labels">Código Postal</label
                ><input
                  type="text"
                  class="form-control"
                  placeholder="Digite o Código Postal"
                  value=""
                />
              </div>
              <div class="col-md-12">
                <label class="labels">Cidade</label
                ><input
                  type="text"
                  class="form-control"
                  placeholder="Digite a cidade"
                  value=""
                />
              </div>
              <div class="col-md-12">
                <label for="inputState" class="form-label">Estado</label>

                <select id="inputState" class="form-select">
                  <option selected>Encontre seu Estado</option>

                  <option value="AC">Acre</option>

                  <option value="AL">Alagoas</option>

                  <option value="AP">Amapá</option>

                  <option value="AM">Amazonas</option>

                  <option value="BA">Bahia</option>

                  <option value="CE">Ceará</option>

                  <option value="DF">Distrito Federal</option>

                  <option value="ES">Espírito Santo</option>

                  <option value="GO">Goiás</option>

                  <option value="MA">Maranhão</option>

                  <option value="MT">Mato Grosso</option>

                  <option value="MS">Mato Grosso do Sul</option>

                  <option value="MG">Minas Gerais</option>

                  <option value="PA">Pará</option>

                  <option value="PB">Paraíba</option>

                  <option value="PR">Paraná</option>

                  <option value="PE">Pernambuco</option>

                  <option value="PI">Piauí</option>

                  <option value="RJ">Rio de Janeiro</option>

                  <option value="RN">Rio Grande do Norte</option>

                  <option value="RS">Rio Grande do Sul</option>

                  <option value="RO">Rondônia</option>

                  <option value="RR">Roraima</option>

                  <option value="SC">Santa Catarina</option>

                  <option value="SP">São Paulo</option>

                  <option value="SE">Sergipe</option>

                  <option value="TO">Tocantins</option>
                </select>
              </div>
              <div class="col-md-12">
                <label class="labels">Email</label
                ><input
                  type="text"
                  class="form-control"
                  placeholder="Digite o email"
                  value=""
                />
              </div>
              <div class="col-md-12">
                <label class="labels">Educação</label
                ><input
                  type="text"
                  class="form-control"
                  placeholder="Digite qual curso tem"
                  value=""
                />
              </div>
            </div>
            <!--<div class="row mt-3"> -->
            <div class="col-md-12">
              <label class="labels">País</label
              ><input
                type="text"
                class="form-control"
                placeholder="Digite o País"
                value=""
              />
            </div>
            <!--<div class="col-md-6">
                <label class="labels">State/Region</label>
                <input type="text" class="form-control" value="" placeholder="state"><
                /div>         
            </div> -->
            <div class="mt-5 text-center">
              <button class="btn btn-primary profile-button" @click="salvar" type="buttom">
                Salve o Perfil
              </button>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="p-3 py-5">
            <div
              class="
                d-flex
                justify-content-between
                align-items-center
                experience
              "
            >
              <span>Editar Experiencia</span
              ><span class="border px-3 p-1 add-experience"
                ><i class="fa fa-plus"></i>&nbsp;Experiencia</span
              >
            </div>
            <br />
            <div class="col-md-12">
              <label class="labels">Experiencia em Projetar</label
              ><input
                type="text"
                class="form-control"
                placeholder="Experiencia"
                value=""
              />
            </div>
            <br />
            <div class="col-md-12">
              <label class="labels">Detalhes adicionais</label
              ><input
                type="text"
                class="form-control"
                placeholder="Digite os detalhes"
                value=""
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


//v-model="test"

<script>
export default {
  name: "Cadastro",
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
      this.axios.get("http://127.0.0.1:8000/teste-view").then((response) => {
        this.data = response.data;
      });
    },
  },
};
</script>