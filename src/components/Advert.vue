<template>
  <aside class="advert">
    <div class="anuncio-item">
      <img src="../assets/anuncio-1.jpg" alt="Anuncios 1" />
    </div>

    <div class="anuncio-item">
      <img src="../assets/anuncio-2.jpg" alt="Anuncios 2" />
    </div>
  </aside>
</template>

<script>
export default {
  name: "AdvertComponent",
};
</script>

<style scoped>
.advert {
  background: #fafbfc;
  display: grid;
  align-content: flex-start;
  padding: 30px;
  grid-gap: 30px;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
}
</style>
