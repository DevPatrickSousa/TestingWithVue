<template>
  <form action="">
    <div>
      <input-text />
    </div>

    <div>
      <input-text />
    </div>

    <div>
      <form-submit />
    </div>
    
  </form>
</template>


<script>
import InputText from "./Form/InputText.vue";
import FormSubmit from "./Form/FormSubmit.vue";
export default {
  name: "FormTeste",
  components: {
    InputText,
    FormSubmit,
  },
};
</script>