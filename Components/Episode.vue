<template>

<div class="container">
        <h2 class="container__subtitle2">épisode {{ id }}</h2>
        <h1 class="container__title">{{ title }}</h1>
        
        <div class="container__imgContainer">
            <h3 class="container__imgContainer__secondTitle">{{ description }}</h3>
            <img class="container__imgContainer__img" alt="img" :src="url"/>
         </div>
         
        </div>

</template>

<script lang="ts" setup>
const props = defineProps({
    id: Number,
    title: String,
    description: String,
    url: String,
});
</script>

<style scoped lang="scss">
.container{
        //position:sticky;
        margin-left: 50px;
        background-color: rgb(255, 196, 0);
        height:220px;
        overflow: visible;
        margin-bottom:80px;

        &__subtitle{
         color:white;
         padding-left: 10px;
        }
        &__subtitle2{
         color:white;
         text-align: right;
         padding-right: 30px;
        }
        &__title{
            font-size: 40px;
        }
        &__imgContainer{
            display:flex;
            &__secondTitle{
            font-size: 60;
            font-weight: bold;
             }
        
             &__img{
                margin-left:30px;
                width:50%;
                height:150px;
             }

            }
    }


    @media(max-width:520px)
{
    .container
    {
        margin-bottom:200px;

}
}
    
</style>