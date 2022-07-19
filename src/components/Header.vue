<template>
  <header class="header">
    <router-link to="/" class="logo">
      <img src="../assets/wildbeast.svg" alt="Wildbeast" />
    </router-link>
    <nav>
      <ul>
        <li><router-link to="/">Sobre</router-link></li>
        <li><router-link to="/">Animais</router-link></li>
        <li><router-link to="/">Contato</router-link></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
};
</script>

<style scoped>
.header {
  background: linear-gradient(135deg, #8844ee, #b07dfb);
  padding: 30px;
  display: grid;
  grid-template-columns: 1fr auto;
  align-items: center;
}

.logo {
  max-width: 200px;
}

nav ul {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

nav a {
  display: block;
  padding: 10px;
  color: #fff;
  font-size: 1.25rem;
  background: rgba(0, 0, 0, 0.1);
  border-radius: 5px;
  transition: 0.1s;
}

nav a:hover {
  background: rgba(0, 0, 0, 0.5);
}

.header li + li {
  margin-left: 30px;
}
</style>
