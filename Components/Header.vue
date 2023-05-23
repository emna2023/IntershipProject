<template>
    <header class="header">
    <h1 class="header__title"> PowerUp</h1>
    <h2 class="header__subtitle">Le fan site par officiel du tout de chainsaw man</h2>
    <nav class="header__nav">
        <ul class="header__nav__list">
            <li class="header__nav__list__onelist">
                 <NuxtLink class="header__nav__list__onelist__link" to="/"> Accueil</NuxtLink></li>
            <li class="header__nav__list__onelist"> 
                <NuxtLink class="header__nav__list__onelist__link" to="/apropos"> A propos</NuxtLink></li>
            <li class="header__nav__list__onelist">
                <NuxtLink class="header__nav__list__onelist__link" to="/contact"> Contact</NuxtLink></li>
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
<style scoped lang="scss" >
.header{
    background-color: rgb(255, 196, 0);
    color:rgb(255, 55, 0);
    font-weight:bold;
    padding-top: 0;
    padding-bottom: 2em;
    margin-top: 0;
    margin-right: 0;
    margin-left: 0;


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
    margin-right: 20px;
    &__list{
        display:flex;
        justify-content: space-between;
        list-style: none;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        &__onelist{
            &__link{
                text-decoration: none;
                color:rgb(255, 55, 0);
            }
            &__link:hover{
            color:antiquewhite;
           }
        }

    }
   }

}
@media(max-width:520px)
{
    .header
    {
        &__subtitle{
    font-size: 20px;
        }
        &__nav{
     &__list{
        display:block;
        
    }
}
}
}
@media(min-width:1000px)
{
    .header
    {
        margin-top: 0;
    margin-left: 0;
    margin-right: 0;

    &__title{
    font-size:3em;
   }
   
   &__subtitle{
    font-size:2em;
   }

        &__nav{
    &__list{
        justify-content: space-between;
        &__onelist{
            &__link{
                font-size: 2em;

            }
        }
    }
}
       
}
}

</style>