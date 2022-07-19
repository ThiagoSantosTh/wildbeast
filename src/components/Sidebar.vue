<template>
  <nav class="sidenav">
    <ul>
      <li>
        <router-link to="/"
          ><img src="../assets/icons/cervo.svg" alt="Cervo"
        /></router-link>
      </li>
      <li>
        <router-link to="/"
          ><img src="../assets/icons/leao.svg" alt="Leão"
        /></router-link>
      </li>
      <li>
        <router-link to="/"
          ><img src="../assets/icons/gato.svg" alt="Gato"
        /></router-link>
      </li>
      <li>
        <router-link to="/"
          ><img src="../assets/icons/vaca.svg" alt="Vaca"
        /></router-link>
      </li>

      <li>
        <router-link to="/"
          ><img src="../assets/icons/ovelha.svg" alt="Ovelha"
        /></router-link>
      </li>

      <li>
        <router-link to="/"
          ><img src="../assets/icons/abelha.svg" alt="Abelha"
        /></router-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "sidebarComponent",
};
</script>

<style scoped>
.sidenav {
  background: #fafbfc;
  padding: 30px;
}

li a {
  display: block;
  min-width: 60px;
  max-width: 100px;
  margin: 0px auto 30px auto;
  background: #fff;
  padding: 20px;
  border-radius: 5px;
  box-shadow: 5px 5px 15px 0px rgba(44, 44, 44, 0.15);
  transition: 0.1s ease-out;
}

li a:hover {
  background: #b07dfb;
}
</style>
