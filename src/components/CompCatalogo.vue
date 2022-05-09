<script>
import ListaProducoes from "./ListaProducoes.vue";

export default {
  components: { ListaProducoes },
  data() {
    return {
      producoes: [
        {
          tipo: "FILMES",
          producoes: [
            {
              nome: "PS! Eu ainda te amo",
              imagem: new URL("./imgs/ps_ainda_amo_voce.jpg", import.meta.url)
                .href,
            },
            {
              nome: "Para todos os garotos que já amei",
              imagem: new URL(
                "./imgs/Para_todos_os_garotos_que_ja_amei_.jpg",
                import.meta.url
              ).href,
            },
            {
              nome: "Barraca do Beijo",
              imagem: new URL("./imgs/barraca do beijo.jpg", import.meta.url)
                .href,
            },
            {
              nome: "Barraca do Beijo 2",
              imagem: new URL("./imgs/barraca do beijo2.jpg", import.meta.url)
                .href,
            },
            {
              nome: "Barraca do Beijo 3",
              imagem: new URL(
                "./imgs/a barraca do beijo 3.jpg",
                import.meta.url
              ).href,
            },
          ],
        },
        {
          tipo: "SÉRIES",
          producoes: [
            {
              nome: "Greys Anatomy",
              imagem: new URL("./imgs/greys anatomy.jpg", import.meta.url).href,
            },
            {
              nome: "Riverdale",
              imagem: new URL("./imgs/riverdale.jpg", import.meta.url).href,
            },
            {
              nome: "Ginny e Georgia",
              imagem: new URL("./imgs/ginny e georgia.jpg", import.meta.url)
                .href,
            },
            {
              nome: "Once upon a time",
              imagem: new URL("./imgs/once upon a time.jpg", import.meta.url)
                .href,
            },
            {
              nome: "Dinastia",
              imagem: new URL("./imgs/dinastia.jpg", import.meta.url).href,
            },
          ],
        },
        {
          tipo: "DORAMA",
          producoes: [
            {
              nome: "Good",
              imagem: new URL("./imgs/good.jpg", import.meta.url).href,
            },
            {
              nome: "To the",
              imagem: new URL("./imgs/to the.jpg", import.meta.url).href,
            },
            {
              nome: "One",
              imagem: new URL("./imgs/one.jpg", import.meta.url).href,
            },
            {
              nome: "Pousando no amor",
              imagem: new URL("./imgs/pousando no amor.jpg", import.meta.url)
                .href,
            },
            {
              nome: "Vicenzo",
              imagem: new URL("./imgs/vicenzo.jpg", import.meta.url).href,
            },
          ],
        },
      ],
    };
  },
};
</script>

<template>
  <ListaProducoes
    v-for="(producao, i) of producoes"
    :key="i"
    :producoes="producao"
  />
</template>
