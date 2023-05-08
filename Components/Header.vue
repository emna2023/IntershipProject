<template>
    <header class="header">
    <h1 class="header__title"> PowerUp</h1>
    <h2 class="header__subtitle">Le fan site par officiel du tout de chainsaw man</h2>
    <nav class="header__nav">
        <ul class="header__nav__list">
            <li class="header__nav__list__onelist">
                 <NuxtLink class="header__nav__list__onelist__link" to="/"> Accueil</NuxtLink></li>
            <li class="header__nav__list__onelist"> 
                <NuxtLink class="header__nav__list__onelist__link" to="/apropos"> Apropos</NuxtLink></li>
            <li class="header__nav__list__onelist">
                <NuxtLink class="header__nav__list__onelist__link" to="/contact"> contact</NuxtLink></li>
            <li class="header__nav__list__onelist">
                <NuxtLink class="header__nav__list__onelist__link" to="/episodes"> Listes des episodes</NuxtLink></li>
            <li class="header__nav__list__onelist">
                <NuxtLink class="header__nav__list__onelist__link" to="/personnages"> Personnages</NuxtLink></li>
        </ul>
    </nav>
    </header>
    </template>
    <script setup>
    
</script>
<style lang="scss" >
.header{
    background-color: rgb(255, 196, 0);
    color:rgb(255, 55, 0);
    font-weight:bold;
    padding-bottom: 2em;


   &__title{
font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
font-size:120 px;
text-align: center;
   }
   &__subtitle{
    font-family: 'Times New Roman', Times, serif;
    text-align: center;
   }
   &__nav{
    &__list{
        display:flex;
        justify-content: space-around;
        list-style: none;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        &__onelist{
            &__link{
                text-decoration: none;
                color:rgb(255, 55, 0);
            }
        }

    }
   }

}
</style>