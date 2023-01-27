<template>
  <div>
    <Message :msg="msg" :msgClass="msgClass" />
    <form
      id="user-form"
      @submit="page === 'register' ? register($event) : update($event)"
    >
      <input type="hidden" id="id" name="id" v-model="id" />
      <div class="input-container">
        <label for="name">Nome:</label>
        <input
          type="text"
          id="name"
          name="name"
          v-model="name"
          placeholder="Digite o seu nome"
        />
      </div>
      <div class="input-container">
        <label for="email">Email:</label>
        <input
          type="email"
          id="email"
          name="email"
          v-model="email"
          placeholder="Digite o seu e-mail"
        />
      </div>
      <div class="input-container">
        <label for="password">Senha:</label>
        <input
          type="password"
          id="password"
          name="password"
          v-model="password"
          placeholder="Digite sua senha"
        />
      </div>
      <div class="input-container">
        <label for="confirmpassword">Confirmação:</label>
        <input
          type="password"
          id="confirmpassword"
          name="confirmpassword"
          v-model="confirmpassword"
          placeholder="Confirme sua senha"
        />
      </div>
      <InputSubmit :text="btnText" />
    </form>
  </div>
</template>

<script lang="ts">
import InputSubmit from "./form/InputSubmit.vue";
export default {
  name: "UserForm",
  components: {
    InputSubmit,
  },
  data() {
    return {
      id: null,
      name: null,
      email: null,
      password: null,
      confirmpassword: null,
      btnText: "Cadastrar",
    };
  }
};

</script>

<style scoped>
.register {
  text-align: center;
  padding-top: 40px;
  padding-bottom: 100px;
}
.register h1 {
  margin-bottom: 40px;
}
</style>
