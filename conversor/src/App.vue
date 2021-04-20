<template>
  <div class="container">
    <h1>Conversor de Moedas</h1>
    <div class="linha">
      <Conversor moeda-a="USD" moeda-b="BRL"/>
      <h3 class="moeda">DOLAR</h3>
      <Conversor moeda-a="BRL" moeda-b="USD"/>
    </div>
    <div class="linha">
      <Conversor moeda-a="EUR" moeda-b="BRL"/>
      <h3 class="moeda">EURO</h3>
      <Conversor moeda-a="BRL" moeda-b="EUR"/>
    </div>
    <div class="linha">
      <Conversor moeda-a="GBP" moeda-b="BRL"/>
      <h3 class="moeda">LIBRA</h3>
      <Conversor moeda-a="BRL" moeda-b="GBP"/>
    </div>
    <div class="linha">
      <Conversor moeda-a="CHF" moeda-b="BRL"/>
      <h3 class="moeda">FRANCO</h3>
      <Conversor moeda-a="BRL" moeda-b="CHF"/>
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";
export default {
  name: 'App',
  components: {
    Conversor
  }
}
</script>

<style>
#app {
  margin: auto;
  max-width: 800px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #021a31;
  margin-top: 60px;
}

.linha {
  display: flex;
  justify-content: space-around;
  margin-top: 15px;
  }

.moeda{
  text-align: center;
  margin: auto;
}

</style>
