<template>
  <h2>meu nome é {{ nome }} e abaixo estão meus dados:</h2>
  <info-data />
  <form-teste />
</template>

<script>
import FormTeste from "./FormTeste.vue";
import InfoData from "./InfoData.vue";
export default {
  name: "PeopleData",
  data() {
    return {
      nome: "Patrick",
    };
  },
  components: {
    InfoData,
    FormTeste,
  },
};
</script>