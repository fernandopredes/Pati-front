<template>
  <nav id="nav">
    <router-link to="/">
      <img src="/img/patilogo.ong" alt="pati">
    </router-link>
    <h2 id="nav-title">Pati</h2>
    <div id="nav" class="links">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/about">Entrar</router-link>
      <router-link to="/register">Cadastrar</router-link>
    </div>
  </nav>
</template>

<script lang="ts">
export default {
  name: "NavbarItem",
};
</script>

<style scoped>
nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px;
  border-bottom: 1px solid #eee;
}
#nav a {
  text-decoration: none;
  margin-right: 15px;
}
#nav img {
  width: 35px;
}
#nav-title {
  font-size: 3rem;
  font-weight: 300;
}
#logo-container,
#nav-links {
  width: 400px;
}
#nav-links {
  display: flex;
  justify-content: flex-end;
}
button {
  background-color: #FFFFFF;
  border: none;
  font-size: 16px;
  cursor: pointer;
}
button:hover {
  color: #c1b696;
}
</style>
