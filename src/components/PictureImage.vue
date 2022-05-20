<template>
    <img :src="avatar" :alt="Logo">
</template>


<script>
export default {
    name:'PictureImage',
    data(){
        return{
            avatar: '/img/avatar.png',
            description: 'Logo'
        }
    }
}
</script>