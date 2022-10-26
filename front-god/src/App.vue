<template>
  <div>
    <Header />
    <PrimeiroComponente />
    <p class="paragrafo_pai">Testando dado de teste: {{ testando }}</p>
    <LifeCycle />
    <Pessoa />
    <Form></Form>
  </div>

</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import Pessoa from './components/Pessoa.vue';
import LifeCycle from './components/LifeCycle.vue';
import Form from './components/Form.vue';
import Header from './components/Header.vue'
export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Form,
    Header
},
  data() {
    return {
      testando: "dado de teste"
    }
  }
};
</script>

<style>
body {
  background-color: #333;
  color: #fff;
}
a {
  color: red;
}

.teste {
  background-color: #000;
}
</style>