<template>
  <img :src="avatar" :alt="Logo" />
  <change-image @Change-Image='changeText'/>
</template>


<script>
import ChangeImage from "./ChangeImage.vue";
export default {
  name: "PictureImage",
  data() {
    return {
      avatar: "/img/avatar.png",
      description: "Logo",
    };
  },
  components: {
    ChangeImage,
  },
  methods:{
      changeText(){
          this.avatar = '/img/postman.png'
      }
  }
};
</script>