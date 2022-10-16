<template>
  <div>
    <PrimeiroComponente />
    <p>Testando dado de teste: {{ testando }}</p>
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
export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Form
},
  data() {
    return {
      testando: "dado de teste"
    }
  }
};
</script>