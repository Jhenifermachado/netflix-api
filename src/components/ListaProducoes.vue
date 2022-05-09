<script>
export default {
  props: ["producoes"],
};
</script>
<template>
  <div class="lista-producoes">
    <div class="container bg-info">
      <h2>{{ producoes.tipo }}</h2>
    </div>
    <div class="container">
      <div class="row">
        <div class="col" v-for="(producao, i) of producoes.producoes" :key="i">
          <img
            :src="producao.imagem"
            width="195"
            height="350"
            class="img-fluid"
            alt="..."
            :title="producao.nome"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.lista-producoes {
  margin-top: 3%;
}
</style>
