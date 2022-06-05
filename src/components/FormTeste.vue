<template>
  <form action="" @submit="SendForm($event)">
    <div>
      <input type="text" :v-model="name" placeholder="teste" />
    </div>

    <div>
      <input type="text" :v-model="email" />
    </div>

    <div>
      <form-submit />
    </div>
  </form>
</template>


<script>

import FormSubmit from "./Form/FormSubmit.vue";
export default {
  name: "FormTeste",
  components: {
    
    FormSubmit,
  },
  data() {
    return {
      name: "asd",
      email: "asd",
    };
  },
  methods: {
    SendForm(e) {

const name = this.name
const email = this.email

      e.preventDefault();

      console.log("Form Enviado");

      console.log('o nome é '+ name)
      console.log('o email é '+ email)
    },
  },
};
</script>