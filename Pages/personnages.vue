<template>
    <main class="main">

        <!-- <div class="main__imgContainer">
            <h1 class="main__imgContainer__title1"> {{ personnes[0].title }} </h1>
            <img class="main__imgContainer__img" alt="img" :src="personnes[0]['@id']"/>
         </div> -->

<!-- appel au component personnage -->
         <Personnage v-for= "personne in personnes" 
         :title="personne.title" 
         :img="personne['@id']" /> 

   
    </main>
</template>

<script lang="ts" setup>

import {Buffer} from 'buffer';
const config = useRuntimeConfig();
//aller a nuxt.config.ts
 const { data: myData } = await useFetch("personnages", {
   baseURL: config.public.apiBase,
   headers: {
     Accept: "application/json",
     Authorization:
       "Basic " +
       Buffer.from("admin:admin").toString("base64"),
   },
 });
 console.log("c'est l'api:" + myData.value);
const personnes = myData.value.items;
</script>

<style scoped lang="scss">
.main{
    margin-right: 0;
    margin-left: 0;

//     &__imgContainer{
//         position:relative;

//         &__img{
// width:100%;

//         }
//         &__title1{
//             position:absolute;
//             text-align:left;
//             margin-left: 30px;
//             font-size: 50px;
//             color:white;
//             font-family: Georgia, 'Times New Roman', Times, serif;

//         }
//         &__title2{
//             position:absolute;
//             right:30px;
//             //text-align:right;
//            // margin-right: 30px;
//             font-size: 50px;
//             color:white;
//             font-family: Georgia, 'Times New Roman', Times, serif;

//         }
        
// }
// &__arraws{
//         display:flex;
//         justify-content: center;
//         align-content: space-around;
//     }
//     &__img{
//         //color:yellow;
//     }
}
</style>