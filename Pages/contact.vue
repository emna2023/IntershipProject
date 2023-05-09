<template>
    <main>
<main class="main">
<h1 class="main__title">  NOUS CONTACTER</h1>
<div class="main____imgContainer">
            <img class="main__imgContainer__img" alt="img1" src="/Media/CONTACTChainsawman.jpg" />

        </div>

    <form class="main__form" method="post" action="">

    <p class="main__form__p">
    <label class="main__form__p__label"> E-mail</label> :
     <input class="main__form__p__input"   type="text" name="mail" /> </p>

    <p class="main__form__p">
    <label class="main__form__p__label">Message</label> : 
    <textarea class="main__form__p__textarea" name="ameliorer" id="ameliorer" rows="8" > </textarea>
     </p>
     <p class="main__form__p">
    <input class="main__form__p__submit" type="submit" value="Envoyer" />   
     </p>

    
</form>




</main>
    </main>
</template>
<script setup>
</script>

<style lang="scss">

.main{
    &__title
    {
        text-align: center;
        font-size: 4em;
    }
    &__form{
        text-align: center;
        &__p{
            &__label{
                font-weight: bold;
                size:80px;
                //position du texte au début du zone de texte ne fonctionne pas
                align-content: flex-start;

            }
            &__textarea{
                background-color: yellow;
            }
            &__input{
                background-color: yellow;

            }
            &__submit{
                color: rgb(255, 119, 0);
                font-weight: bolder;
            }

        }
    }}
</style>