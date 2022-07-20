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

@keyframes seta {
  from {
    right: 30px;
  }
  to {
    right: 20px;
  }
}

@media (max-width: 760px) {
  .sidenav ul {
    display: flex;
  }
  .sidenav li {
    flex: 1 0 60px;
  }
  .sidenav {
    padding: 0 30px;
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    position: relative;
  }

  .sidenav li a {
    margin: 30px 30px 30px 0;
  }
  .sidenav::after {
    content: "→";
    position: absolute;
    top: 5px;
    right: 30px;
    color: rgba(0, 0, 0, 0.3);
    animation: seta 0.5s ease-in 0s infinite alternate;
  }
}
</style>
