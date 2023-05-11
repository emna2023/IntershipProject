<template>
    <main class="main">
        <div class="main__imgContainer">
            <h1 class="main__imgContainer__title1"> MAKIMA </h1>
            <img class="main__imgContainer__img" alt="img" src="/Media/Chainsaw-Man-Makima-2.webp"/>

      </div>
      
      <div class="main__imgContainer">
        <h1 class="main__imgContainer__title2">DENJI</h1>

            <img class="main__imgContainer__img" alt="img" src="/Media/DENJI.png"/>
      </div>
      <div class="main__arraws">
            <img class="main__arraws__img" alt="arrawBack" src="/Media/arrow_back.png"/>
            <img class="main__arraws__img" alt="arrawNext" src="/Media/arrow_follow.png">
        </div>


    </main>
</template>

<script setup>
</script>

<style scoped lang="scss">
.main{
    margin-right: 0;
    margin-left: 0;

    &__imgContainer{
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
            font-family: Georgia, 'Times New Roman', Times, serif;

        }
        &__title2{
            position:absolute;
            right:30px;
            //text-align:right;
           // margin-right: 30px;
            font-size: 50px;
            color:white;
            font-family: Georgia, 'Times New Roman', Times, serif;

        }
        
}
&__arraws{
        display:flex;
        justify-content: center;
        align-content: space-around;
    }
    &__img{
        //color:yellow;
    }
}
</style>