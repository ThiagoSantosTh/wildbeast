<template>
  <main class="content">
    <div class="titulo">
      <h1>Lobo Cinza</h1>
      <span>da família canis lupus</span>
    </div>

    <div class="caracteriscticas">
      <div>
        <span class="numero">72</span>
        <span class="rotulo">kg</span>
      </div>
      <div>
        <span class="numero">13</span>
        <span class="rotulo">age</span>
      </div>
    </div>

    <p class="col-wide">
      É um sobrevivente da Era do Gelo, originário do Pleistoceno Superior,
      cerca de 300 mil anos atrás.[2] O sequenciamento de DNA e estudos
      genéticos reafirmam que o lobo cinzento é ancestral do cão doméstico.
    </p>

    <img class="imagem-1" src="../assets/wolf1.jpg" alt="Wolf 1" />
    <p class="destaque">
      É um sobrevivente da Era do Gelo, originário do Pleistoceno Superior,
      cerca de 300 mil anos atrás.[2] O sequenciamento de DNA e estudos.
    </p>

    <img class="imagem-2" src="../assets/wolf2.jpg" alt="Wolf 2" />
    <p>
      O peso e tamanho dos lobos variam muito em todo o mundo, tendendo a
      aumentar proporcionalmente com a latitude, como previsto pela teoria de
      Christian Bergmann. Em geral, a altura, medida a partir dos ombros, varia
      de 60 a 95 centímetros.
    </p>

    <p>
      O peso varia geograficamente. Em média, os lobos europeus pesam 38,5 kg;
      os lobos da América do Norte, 36 kg; os lobos indianos e árabes, 25 kg.[7]
      Embora raros, lobos com mais de 77 kg foram encontrados no Alasca,
      Canadá,[8] e na antiga União Soviética.
    </p>

    <blockquote class="col-wide citacao">
      <p>
        “Há algo no uivar do lobo que tira um homem do aqui e agora e o
        transporta para uma floresta da mente.”
      </p>
    </blockquote>

    <ul class="atributos">
      <li>Surgiu: 12.000 anos</li>
      <li>Tipo: Mamífero</li>
      <li>Macho adulto: 80kg</li>
      <li>Fêmea adulta: 55kg</li>
      <li>Família: Lupus</li>
    </ul>

    <div class="informacoes">
      <p>
        É um sobrevivente da Era do Gelo, originário do Pleistoceno Superior,
        cerca de 300 mil anos atrás.[2] O sequenciamento de DNA e estudos
        genéticos reafirmam que o lobo cinzento é ancestral do cão doméstico.
      </p>

      <p>
        É um sobrevivente da Era do Gelo, originário do Pleistoceno Superior,
        cerca de 300 mil anos atrás.[2] O sequenciamento de DNA e estudos
        genéticos reafirmam que o lobo cinzento é ancestral do cão doméstico.
      </p>
    </div>

    <img class="col-wide" src="../assets/wolf3.jpg" alt="Wolf 3" />
  </main>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style scoped>
.content {
  max-width: 900px;
  margin: 0 auto;
  padding: 30px;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 30px;
}

.imagem-1 {
  grid-row: span 2;
  align-self: flex-end;
}

.imagem-2 {
  align-self: flex-end;
}

.informacoes p + p {
  margin-top: 30px;
}

.titulo {
  color: #b07dfb;
}

.titulo h1 {
  font-size: 3.75em;
  line-height: 1;
  font-weight: 700;
}

.titulo span {
  font-size: 0.875em;
  font-style: italic;
}

.caracteriscticas {
  display: flex;
  align-items: flex-start;
}

.caracteriscticas > div {
  width: 80px;
  text-align: center;
  background: linear-gradient(135deg, #8844ee, #b07dfb);
  border-radius: 5px;
  box-shadow: 5px 5px 15px 0px rgba(44, 44, 44, 0.15);
  position: relative;
}

.caracteriscticas > div:first-child {
  margin-right: 30px;
}

.caracteriscticas span {
  display: block;
  color: #b07dfb;
}

.numero {
  font-size: 3em;
  line-height: 1;
  margin: 10px auto;
}

.rotulo {
  background: white;
  border-radius: 0 0 5px 5px;
  padding: 5px 0;
  position: relative;
  top: 2px;
}

.destaque {
  font-size: 0.875em;
  color: #b07dfb;
  max-width: 16em;
}

.citacao,
.atributos {
  align-self: start;
  padding: 30px;
  border-radius: 5px;
  box-shadow: 5px 5px 15px 0px rgba(44, 44, 44, 0.15);
  background: linear-gradient(135deg, #8844ee, #b07dfb);
}

.citacao p {
  font-size: 1.5em;
  font-style: italic;
  text-align: center;
  max-width: 500px;
  margin: 0 auto;
  color: white;
}

.atributos li {
  color: white;
  font-family: Courier, monospace;
  font-size: 1.125em;
  padding: 15px;
}

.atributos li + li {
  border-top: 2px solid #b07dfb;
}

@media (max-width: 600px) {
  .content {
    grid-template-columns: auto;
  }
}
</style>
