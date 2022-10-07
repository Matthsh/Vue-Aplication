<template>
  <div>
    <PrimeiroComponente />
    <p>Testando dado de teste: {{ testando }}</p>
    <LifeCycle />
  </div>

</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
export default {
  name: "App",
  components: { PrimeiroComponente, LifeCycle },
  data() {
    return {
      testando: "dado de teste"
    }
  }
};
</script>