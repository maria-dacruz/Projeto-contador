<template>
  <div class="Novo">
    <h1>Contador</h1>
    <div class="sub">
      <P>Clique para subtrair: </P><button v-on:click="Subtrair">-</button>
    </div>
    <div class="sum">
      <p>Clique para somar: </p>
      <button v-on:click="Somar">+</button>
    </div>

    <p><strong>Valor atual:</strong> {{ mensagem }}</p>
  </div>
</template>

<script>
export default {
  name: "ProjContador",
  data() {
    return {
      mensagem: 0,
    };
  },
  methods: {
    Somar() {
      this.mensagem = this.mensagem + 1;
    },
    Subtrair() {
      this.mensagem = this.mensagem - 1;
    },
  },
};
</script>

<style scoped>
.sub {
  display: flex;
  padding: 5px;
 justify-content: center;
}
.sum {
    padding: 5px;
    display: flex;
    justify-content: center;
}
</style>