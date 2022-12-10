<template>
  <div id="app">
    <div class="text-center text-warning">
      <h1>
        Conversor de moedas
        <span class="fa fa-money text-success" arial-hidden="true"></span>
      </h1>
      <p class="text-secondary">
        Este é um simples projeto de conversor de moedas para desenvolvimento
        pessoal.
      </p>
    </div>
    <div class="container">
      <Conversor moneyB="BRL" moneyA="USD" />
      <Conversor moneyB="USD" moneyA="BRL" />
    </div>
    <div class="container">
      <Conversor moneyB="BRL" moneyA="EUR" />
      <Conversor moneyB="EUR" moneyA="BRL" />
    </div>
    <div class="container">
      <Conversor moneyB="BRL" moneyA="CAD" />
      <Conversor moneyB="CAD" moneyA="BRL" />
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";
export default {
  name: "app",
  components: {
    Conversor,
  },
};
</script>

<style scoped>

.container {
  display: flex;
  justify-content: space-around;
  margin-bottom: 25px;
}
.text-center {
  margin-bottom: 60px;
  margin-top: 30px;
}
@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
