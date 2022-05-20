<template>
    <h1>meu nome é {{nome}}</h1>
</template>

<script>
export default {
    name:'LifeCycle',
    data()
    {
        return{
            nome:'Aguardando a criação do componente!!!'
        }
    },
    created(){
        setTimeout(()=>{
        this.nome = 'Componente criado!'
        }, 1000)
        this.lifeCycle()
        
    },
    mounted(){
        setTimeout(()=>{
        this.nome = 'Patrick Sousa'
        }, 2000)
        this.lifeCycle()
    },
    methods:{
        lifeCycle(){
            console.log('executou')
        }
    }
}
</script>
