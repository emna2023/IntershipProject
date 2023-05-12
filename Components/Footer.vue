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
                <NuxtLink class="footer__w__container__nav__list__onelist__link" to="/contact"> Contact</NuxtLink></li>
            <li class="footer__w__container__nav__list__onelist">
                <NuxtLink class="footer__w__container__nav__list__onelist__link" to="/episodes"> Listes des episodes</NuxtLink></li>
            <li class="footer__w__container__nav__list__onelist">
                <NuxtLink class="footer__w__container__nav__list__onelist__link" to="/personnages"> Personnages</NuxtLink></li>
        </ul>
    </nav>
</div>
    <div class="footer__w__secondContainer">
        <!-- <img class="footer__w__secondContainer__img" alt="img1" src="../public/Media/3wp9532701.jpeg"/> -->
    </div>

</div>


</footer>
</template>

<style lang="scss" >
h1,h2{
font-family: 'Righteous', cursive;

}

.footer{
    background-color: rgb(255, 196, 0);
    color:rgb(255, 55, 0);
    font-weight:bold;
    margin-bottom: 0;
    margin-left: 0;
    margin-right: 0;
       &__title{
        padding-left: 30px;
       }
        &__w{
        display:grid;
        grid-template-columns: 70% 30%;
        //display:flex;
        justify-content: space-between;
      &__container{
             &__nav{
                &__list{
                  display:block;

                     list-style: none;
                     text-decoration: none;
                    &__onelist{
                        margin-bottom: 5px;
                      &__link{
                      text-decoration: none;
                     color:rgb(255, 55, 0);

                            }
                            &__link:hover{
                     background-color:black;

                               }
                        }
                        }
                                }
                    }

    &__secondContainer{
        
        width: 250px;
        height: 180px;
        background-image: url("/Media/3wp9532701.jpeg");
        background-size: cover;
        //mix-blend-mode: overlay;
        //isolation: isolate;

        //background-color: transparent;
       // background-color: rgb(255, 196, 0);




        
    // &__img{
    //     max-width:50%;
    //     position: relative;
    //     isolation: isolate;


        //position: absolute;

        
    }
    // &__img::after{
    //     content:"";
    //     display: block;
    //     position: absolute;
    //     top:0;
    //     left:0;
    //     width:100%;
    //     height:100%;
    //     mix-blend-mode: screen;
    //     background-color: transparent;
    // }
   }
}

@media(max-width:520px)
{
    .footer
    {
        font-size: larger;
        
    }
}

@media(min-width:1000px)
{
   .footer{
    &__title{
        font-size: 4em;
    }
   &__w{
        &__container{
             &__nav{
                &__list{
                   &__onelist{
                      &__link{

                       font-size: 20px;
                      }
                    }
                }
            }
        }
    }
}}
</style>