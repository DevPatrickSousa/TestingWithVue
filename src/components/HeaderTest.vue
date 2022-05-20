<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Home</a></li>
        <li><a href="#">Home</a></li>
    </ul>
</template>

<script>
export default {
    name:'HeaderTest'
}
</script>

<style scoped>
ul{
    list-style: none;
    display: flex;
    background-color: blue;
}
li{
    margin-right: 10px;
    color: black;
}
a{
    color: #FFF;
    text-decoration: none;
    transition: .5ms;
}
a:hover{
    color: rgb(224, 64, 184);
}
</style>