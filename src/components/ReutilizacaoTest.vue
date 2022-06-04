<template>
    <button @click="activate">click here!</button>

<span v-show="ativou">Ativado!</span>

</template>

<script>
export default {
    name:'ReutilizacaoTest',
    data(){
        return{
            ativou:false
        }
    },
    methods:{
        activate(){
            this.ativou = !this.ativou
        }
    }
}
</script>