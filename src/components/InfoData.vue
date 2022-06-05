<template>
  <p>
    {{ compEmail }}
  </p>

  <p v-if="esta_estudando">o que estou aprendendo no momento:</p>
  <p v-else>não estou estudando</p>
  <ul>
    <li v-for="(technology, index) in myTechnologies" :key="index">
      {{ myTechnologies }}
    </li>
  </ul>
  <p></p>

  <ul>
    <li v-for="technology in frontEndTechnologies" :key="technology">
      {{ technology.language }}
    </li>
  </ul>
  <div>
    <button @click="showEmail">{{ textoBotao }}</button>
  </div>
  <p v-show="mostra_email">o meu e-mail é: {{ email }}</p>
  <p><a v-bind:href="github" target="_blank">github</a></p>
  <PictureImage />
</template>

<script>
import PictureImage from "./PictureImage.vue";
export default {
  name: "InfoData",
  data() {
    return {
      esta_estudando: true,
      mostra_email: false,
      github: "https://github.com/DevPatrickSousa",
      textoBotao: "Mostrar e-mail",
      myTechnologies: ["HTML", "CSS", "JavaScript", "Vuejs"],
      frontEndTechnologies: [
        { id: 1, language: "HTML" },
        { id: 2, language: "CSS" },
        { id: 3, language: "JAVASCRIPT" },
      ],
    };
  },
  props: {
    email: String,
  },
  components: {
    PictureImage,
  },
  methods: {
    showEmail() {
      this.mostra_email = !this.mostra_email;
      if (!this.mostra_email) {
        this.textoBotao = "mostrar e-mail";
      } else {
        this.textoBotao = "ocultar e-mail";
      }
    },
  },
};
</script>