<template>
  <div>
    <h1>Olá Vue</h1>
    <p>meu nome é {{ nome }}</p>
    <reutilizacao-test/>
    <reutilizacao-test/>
    <reutilizacao-test/>
    <MultiEvents />
  </div>
</template>

<script>
import MultiEvents from "./MultiEvents.vue";
import ReutilizacaoTest from './ReutilizacaoTest.vue'
export default {
  name: "FirstComponent",
  data() {
    return {
      nome: "Patrick",
    };
  },
  components: {
    MultiEvents,ReutilizacaoTest
  },
};
</script>