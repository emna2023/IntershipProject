<template>
    <header class="header">
    
    <h1 class="header__title"> PowerUp</h1>
    <h2 class="header__subtitle">Le fan site par officiel du tout de chainsaw man</h2>
    <nav class="header__nav">
        <ul class="header__nav__list">
            <li class="header__nav__list__onelist">Accueil</li>
            <li class="header__nav__list__onelist">A-propos</li>
            <li class="header__nav__list__onelist">Contact</li>
            <li class="header__nav__list__onelist">Liste-des épisodes</li>
            <li class="header__nav__list__onelist">Personnages</li>
        </ul>
    </nav>
    
    </header>
    </template>
    <script setup>
</script>
<style lang="scss" >
.header{
    background-color: rgb(255, 251, 0);

   &__title{
font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
font-size:120 px;
color:rgb(255, 55, 0);
text-align: center;
   }
   &__subtitle{
    font-family: 'Times New Roman', Times, serif;
    color:rgb(255, 55, 0);
    text-align: center;
   }
   &__nav{
    &__list{
        display:flex;
        justify-content: space-around;

    }
   }

}
</style>