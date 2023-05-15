<template>
    <main>
<main class="main">
<h1 class="main__title">  NOUS CONTACTER</h1>
<div class="main__imgContainer">
            <!-- <img class="main__imgContainer__img" alt="img1" src="/Media/CONTACTChainsawman.jpg" /> -->
</div>
    <form class="main__form" method="post" action="">
    <p class="main__form__p">
    <label class="main__form__p__label">   E-mail:   </label> 
    <input class="main__form__p__input"   type="email" name="mail"  size="43"/>
    </p>

    <p class="main__form__p">
    <label class="main__form__p__label">Message:</label> 
    <textarea class="main__form__p__textarea" name="ameliorer" id="ameliorer"  rows="10" cols="40" > </textarea>
     </p>

     <p class="main__form__p">
    <input class="main__form__p__submit" type="submit" value="ENVOYER" />   
     </p>

    
</form>




</main>
    </main>
</template>
<script setup>
</script>

<style lang="scss">

.main{
    margin-right: 0;
    margin-left: 0;
    &__title
    {
        text-align: center;
        font-size: 4em;
        font-weight: bold;
    }
    &__imgContainer
    {
        
        background-image: url("/Media/CONTACTChainsawman.jpg") ;
        background-attachment: fixed; /* Fixe l'image pendant le scroll */
        background-size: cover; /* L'image prendra 100% de l'espace, quitte à la crop */
        background-position: center; /* Centre la position de l'image */
        background-repeat: no-repeat; /* Empêche l'image de se répéter en fonction de la taille d'écran */
        height: 800px; /* On fixe une grande hauteur pour voir plus facilement le scroll */
        
         
    }

    &__form{
        text-align: center;
        &__p{
            &__label{
                font-weight: bold;
                font-size:20px;
                //position du texte au début du zone de texte ne fonctionne pas
                //text-align: center;
                vertical-align:top;


                

            }
            &__textarea{
                background-color:  rgb(255, 196, 0);
                border-color:  rgb(255, 196, 0);


            }
            &__input{
                background-color:  rgb(255, 196, 0);
                border-color:  rgb(255, 196, 0);


            }
            &__submit{
                color:rgb(255, 55, 0);
                font-weight: bold;
                font-size: 30px;
                font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
                border: none;
                background-color: transparent;
            }

        }
    }}
</style>