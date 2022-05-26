<template>
  <div class="final">
    <div :class="`final-texto ${etapa}`">Parabéns :)</div>
    <button class="final-botao" v-on:click="jogarNovamente">
      Jogar novamente
    </button>
  </div>
</template>

<script>
export default {
  name: "Final",
  props: {
    etapa: String,
    texto: String,
    jogarNovamante: Function,
  },
  data() {
    return {};
  },
  methods: {},
  components: {},
};
</script>

<style scoped>
.final-texto {
  margin: 20px 0px;
  font-size: 24px;
  font-weight: bold;
}

.final-texto.enforcado {
  color: rgb(228, 30, 63);
}

.final-texto.ganhador {
  color: rgb(46, 221, 99);
}
</style>
