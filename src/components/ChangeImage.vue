<template>
<div>
  <button @click="$emit('changeImage')">change profile image</button>
  </div>
</template>

<script>
export default {
  name: "ChangeImage",
  emits: ["changeImage"],
};
</script>