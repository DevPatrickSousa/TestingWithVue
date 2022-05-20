<template>
  <div>
    <h1>Olá Vue</h1>
    <p>meu nome é {{ nome }}</p>
  </div>
</template>

<script>
export default {
  name: "FirstComponent",
  data() {
    return{
        nome: 'Patrick'
    }
  }
};
</script>