<template>
    <main class="main">
       
        <div class="main__container">
        <h2 class="main__container__subtitle">épisode 1</h2>
        <h1 class="main__container__title">LE CHIEN ET LA TRONCONNEUSE</h1>
        
        <div class="main__container__imgContainer">
            <img class="main__container__imgContainer__img" alt="img" src="/Media/Chainsaw-Man-chien.jpg"/>
            <h3 class="main__container__imgContainer__secondTitle">Chapitre 1</h3>

         </div>
        </div>

        <div class="main__container">
        <h2 class="main__container__subtitle">épisode 2</h2>
        <h1 class="main__container__title">ARRIVEE A TOKYO</h1>
        
        <div class="main__container__imgContainer">
            <h3 class="main__container__imgContainer__secondTitle">Chapitres 2-3-4-5</h3>

            <img class="main__container__imgContainer__img" alt="img" src="/Media/Chainsaw-Tokyo.jpg"/>

         </div>
        </div>
        <div class="main__arraws">
            <img alt="arrawBack" src="/Media/arrow_back.png"/>
            <img alt="arrawNext" src="/Media/arrow_follow.png">
        </div>

      
</main>
</template>

<script setup>

</script>


<style lang="scss">

.main{
    &__container{
        background-color: rgb(255, 196, 0);
        height:220px;
        overflow: visible;
        margin-bottom: 80px;
        &__subtitle{
         color:white;
        }
        &__title{
            font-size: 30px;
        }
        &__imgContainer{

            display:flex;
            justify-content: space-around;
            &__secondTitle{
            font-size: 40;
            font-weight: bold;
             }
        
             &__img{
             height:150px;
        }

        }


    }
    &__arraws{
        display:flex;
        justify-content: center;
        align-content: space-around;
    }
}



</style>