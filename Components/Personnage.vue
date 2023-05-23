<template>
     <div class="imgContainer">
       <h1 class="imgContainer__title1">  {{title}} </h1>
       <img class="imgContainer__img" alt="img" :src="img"/>
      </div>
</template>


      <script lang="ts" setup>
       const props = defineProps({
        title: String,
        img: String
    });
      </script>


      <style scoped lang="scss">
       .imgContainer{
        position:relative;

        &__img{
width:100%;

        }
        &__title1{
            position:absolute;
            text-align:left;
            margin-left: 30px;
            font-size: 50px;
            color:white;
            font-family: Georgia, 'Times New Roman';
    
        }}
            </style>