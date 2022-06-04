<template>
  <div>
    <button @click="first($event), second($event)">Ativar Multiplos Eventos</button>
    <p>{{multiplos_eventos}}</p>
  </div>
</template>

<script>
export default {
  name: "MultiEvents",
  data() {
    return {
      multiplos_eventos: "",
    };
  },
  methods: {
    first(e) {
      this.multiplos_eventos = "Primeiro evento ativado!";
      e.preventDefault();
    },
    second(e){
        setTimeout(() => {
            this.multiplos_eventos = 'Segundo evento ativado!'
            e.preventDefault();
        }, 1000);
    }
  },
};
</script>

<style scoped>
div {
  margin: 100px;
}
</style>