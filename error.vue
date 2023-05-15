<template>
<div class="container">
    <p>Le code de l'erreur est: {{ error.statusCode }}</p>
    <p>Oups</p>
    <p>{{ error.message }}</p>
</div>
<img alt="img" src="/Media/error.jpg"/>

</template>
<script setup>
defineProps(['error'])
</script>
<style lang="scss">
img{
    width:100%;
}
.container{
    width: 400;
    height:400;
    background-color: aqua;
    font-family: 'Courier New', Courier, monospace;
    font-weight: bolder;
    text-align: center;
}
</style>