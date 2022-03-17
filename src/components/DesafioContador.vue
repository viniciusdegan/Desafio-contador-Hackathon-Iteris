<template>
  <div class="desafio-contador">
    <h1>Contador: {{ contador }}</h1>
    <!-- Definindo o número a ser inserido pelos botões -->

    <button @click="somar">+</button>
    <button @click="subtrair">-</button>
    <!-- Inserindo a funcionalidade de click para somar e subtrair o número -->
  </div>
</template>

<script>
export default {
  name: "DesafioContador",

  data() {
    return {
      contador: 0,
    };
  },
  methods: {
    subtrair() {
      this.contador--;
    },
    somar() {
      this.contador++;
    },
  },
}
</script>
<!-- O Script contém as funções para somar e subtrair o valor 1 do contador definido no HTML -->

<style scoped>
</style>