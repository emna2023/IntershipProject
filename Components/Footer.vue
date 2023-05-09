<template>
<footer class="footer">

<h1 class="footer__title">PowerUp</h1>
<div class="footer__w">

    <div class="footer__w__container">

    <nav class="footer__w__container__nav">
        <ul class="footer__w__container__nav__list">
            <li class="footer__w__container__nav__list__onelist">
                 <NuxtLink class="footer__w__container__nav__list__onelist__link" to="/"> Accueil</NuxtLink></li>
            <li class="footer__w__container__nav__list__onelist"> 
                <NuxtLink class="footer__w__container__nav__list__onelist__link" to="/apropos"> Apropos</NuxtLink></li>
            <li class="footer__w__container__nav__list__onelist">
                <NuxtLink class="footer__w__container__nav__list__onelist__link" to="/contact"> contact</NuxtLink></li>
            <li class="footer__w__container__nav__list__onelist">
                <NuxtLink class="footer__w__container__nav__list__onelist__link" to="/episodes"> Listes des episodes</NuxtLink></li>
            <li class="footer__w__container__nav__list__onelist">
                <NuxtLink class="footer__w__container__nav__list__onelist__link" to="/personnages"> Personnages</NuxtLink></li>
        </ul>
    </nav>
</div>
    <div class="footer__w__secondContainer">
        <img class="footer__w__secondContainer__img" alt="img1" src="../public/Media/3wp9532701.jpeg"/>
    </div>
</div>

</footer>
</template>

<style lang="scss" >
h1,h2{
//font-family: Georgia, 'Times New Roman', Times, serif;
font-family: 'Righteous', cursive;
}
.footer__w__secondContainer:after{
    content:"";
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background-color: transparent;
}
.footer{
    background-color: rgb(255, 196, 0);
    color:rgb(255, 55, 0);
    font-weight:bold;
    padding-bottom: 2em;
    &__w{
        display:grid;
        grid-template-columns: 50% 50%;
        justify-content: space-between;
      &__container{
             &__nav{
                &__list{
                  display:block;
                     list-style: none;
                     text-decoration: none;
                    &__onelist{
                      &__link{
                      text-decoration: none;
                     color:rgb(255, 55, 0);

                            }
                                }

                                }
                    }
                }

     &__secondContainer{
        position: relative;
        
    &__img{
        max-width:20%;
        // pour enlever la couleur d'arriére plan
        background :transparent;
        background-image: none;
        background-image: rgb(255, 55, 0);

    }
   }
}
}


</style>