<template>
    <main class="main">
        <div class="main__imgContainer">
            <img class="main__imgContainer__img" alt="img" src="/Media/Chainsaw-Man-Makima-2.webp"/>
            <h1 class="main__imgContainer__title" >MAKIMA</h1>
      </div>
      
      <div class="main__imgContainer">
            <img class="main__imgContainer__img" alt="img" src="/Media/DENJI.png"/>
            <h1 class="main__imgContainer__title">DENJI</h1>
      </div>


    </main>
</template>

<script setup>
</script>

<style lang="scss">
.main{

    &__imgContainer{
        &__img{

            position:relative;


        }
        &__title{
            padding-top: 20px;
            position:absolute;

        }
    }


}
</style>