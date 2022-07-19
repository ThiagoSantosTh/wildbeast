<template>
  <header class="header">
    <router-link to="/" class="logo">
      <img src="../assets/wildbeast.svg" alt="Wildbeast" />
      <nav>
        <ul>
          <li><router-link to="/">Sobre</router-link></li>
          <li><router-link to="/">Animais</router-link></li>
          <li><router-link to="/">Contato</router-link></li>
        </ul>
      </nav>
    </router-link>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
};
</script>

<style scoped></style>
