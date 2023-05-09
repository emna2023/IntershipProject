<template>
    <main class="main">

<div id="carroussel">
        <div class="main__container">
            <img class="main__container__img" alt="img1" src="../public/Media/1Power bandw.jpg" />
        </div>
        <div class="main__container">
            <img class="main__container__img" alt="img1" src="/Media/DENJI.png" />
        </div>
        <div class="main__container">
            <img class="main__container__img" alt="img1" src="/Media/Chainsaw-Tokyo.jpg" />
        </div>

        <!-- voir ce site pour le carroussel 
        https://www.studio-jag.com/guides/8-meilleurs-carrousels-en-css3-htm5-js-pour-site-web-moderne/ -->


</div>

        <div class="main__secondcontainer"> 
        <h2 class="main__secondcontainer__subtitle">Dernier épisode:</h2>
        <h1 class="main__secondcontainer__title">katana VS TRONCONNEUSE</h1>
        <ul>

        <li><div class="main__secondcontainer__imgcontainer">
            <img class="main__secondcontainer__imgcontainer__img" alt="img1" src="../public/Media/2Chainsaw-Man.jpg" />
        </div></li>
        <li>        <h2 class="main__secondcontainer__subtitle2">Chapitres 35-36-37-38-40</h2></li>

    </ul>

    </div>
    </main>
</template>
<script setup>
</script>

<style lang="scss">
// #carousel
//   position: relative;
//   height: 400px;
//   top: 50%;
//   transform: translateY(-50%);
//   overflow: hidden;
ul{
    display: grid;
    grid-template-columns: 70% 30%;
    list-style: none;
}

.main{

    width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
    &__container{
        &__img{
            width: 100%;
           // object-fit: cover;
        }
    }
        &__secondcontainer{
             width:90%;
             height: 280px;
             overflow:visible;

            background-color: rgb(255, 196, 0);
            position:relative;
            &__subtitle{
                color:white;
            }
            &__imgcontainer{
                &__img{
                    position:absolue;
                    width:70%;
                    
                }
        }
    }
}


</style>