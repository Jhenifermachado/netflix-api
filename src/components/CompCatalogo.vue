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
              nome: "vingadores",
              imagem: new URL("./imgs/vingadores.png", import.meta.url).href,
            },
            {
              nome: "mulan",
              imagem: new URL("./imgs/mulan.jpeg", import.meta.url).href,
            },
            {
              nome: "emchamas",
              imagem: new URL("./imgs/emchamas.jpeg", import.meta.url).href,
            },
            {
              nome: "Barraca do Beijo 2",
              imagem: new URL("./imgs/barraca do beijo2.jpg", import.meta.url)
                .href,
            },
            {
              nome: "xmen",
              imagem: new URL("./imgs/xmen.jpeg", import.meta.url).href,
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
