<template>
  <div id="app">
    <Header></Header>
    <router-view></router-view>
    <Sidebar></Sidebar>
    <Footer></Footer>
    <Advert></Advert>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Sidebar from "./components/Sidebar.vue";
import Footer from "./components/Footer.vue";
import Advert from "./components/Advert.vue";

export default {
  components: {
    Header,
    Sidebar,
    Footer,
    Advert,
  },
};
</script>

<style>
* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

body {
  font-family: "Vollkorn", Georgia, serif;
}

li {
  list-style: none;
}

a {
  text-decoration: none;
}

img {
  max-width: 100px;
}

#app {
  display: grid;
  grid-template-columns: minmax(160px, 1fr) 3fr 300px;
  grid-template-areas:
    "header header header"
    "sidebar content advert"
    "footer footer footer";
}

.header {
  grid-area: header;
}

.sidebar {
  grid-area: sidebar;
}

.content {
  grid-area: content;
}

.footer {
  grid-area: footer;
}

.advert {
  grid-area: advert;
}
</style>
