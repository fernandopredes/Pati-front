<template>
  <footer>
    <h3>Pati &copy; 2023</h3>
    <p>Compartilhando festas com você</p>
  </footer>
</template>

<script lang="ts">
export default {
  name: "FooterItem",
};

function formatDate(date: Date) {
  let ano = date.getFullYear();
  return `${ano}`;
}

let hoje = new Date();

formatDate(hoje);
</script>

<style scoped>
footer {
  background-color: #25282e;
  height: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
footer h3 {
  color: #FFF;
  margin-bottom: 15px;
  font-weight: 300;
  font-size: 1.6rem;
}
footer p {
  color: #c1b696;
}
</style>
