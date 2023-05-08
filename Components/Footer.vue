<template>
<footer class="footer">

<h1 class="footer__title">PowerUp</h1>
<div class="footer__wrapper">

    <nav class="footer__nav">
        <ul class="footer__nav__list">
            <li class="footer__nav__list__onelist">
                 <NuxtLink class="footer__nav__list__onelist__link" to="/"> Accueil</NuxtLink></li>
            <li class="footer__nav__list__onelist"> 
                <NuxtLink class="footer__nav__list__onelist__link" to="/apropos"> Apropos</NuxtLink></li>
            <li class="footer__nav__list__onelist">
                <NuxtLink class="footer__nav__list__onelist__link" to="/contact"> contact</NuxtLink></li>
            <li class="footer__nav__list__onelist">
                <NuxtLink class="footer__nav__list__onelist__link" to="/episodes"> Listes des episodes</NuxtLink></li>
            <li class="footer__nav__list__onelist">
                <NuxtLink class="footer__nav__list__onelist__link" to="/personnages"> Personnages</NuxtLink></li>
        </ul>
    </nav>
    <div class="footer__container">
        <img class="footer__container__img" alt="img1" src="../public/Media/3wp9532701.jpeg"/>
    </div>
</div>

</footer>
</template>

<style lang="scss" >
h1,h2{
//font-family: Georgia, 'Times New Roman', Times, serif;
font-family: 'Righteous', cursive;
}
.footer{
    background-color: rgb(255, 196, 0);
    color:rgb(255, 55, 0);
    font-weight:bold;
    padding-bottom: 2em;
    &__wrapper{
        display:block;
    }

    &__nav{
    &__list{
        display:block;
        list-style: none;

    }
   }
   &__container{
    &__img{
        width:20%;

    }
   }
}

</style>