<template>
   
<main class="main">
<!-- <h1 class="main__title">  NOUS CONTACTER</h1> -->

<h1 class="main__title">{{ myData.id }} </h1>

<div class="main__imgContainer">
            <!-- <img class="main__imgContainer__img" alt="img1" src="/Media/CONTACTChainsawman.jpg" /> -->
</div>
    <form @submit.prevent="sendEmail" class="main__form" method="post" action="">
    <p class="main__form__p">
    <label class="main__form__p__label">   E-mail:   </label> 
    <input class="main__form__p__input"  id="mail"  type="email" name="mail"  size="43"/>
    </p>

    <p class="main__form__p">
    <label id="msg" class="main__form__p__label">Message:</label> 
    <textarea class="main__form__p__textarea" name="ameliorer" id="ameliorer"  rows="10" cols="40" > </textarea>
     </p>

     <p class="main__form__p">
    <button class="main__form__p__submit" id="envoyer" type="submit">Envoyer</button>  
     </p>

    
</form>




</main>

</template>
<script lang="ts" setup>
import {Buffer} from 'buffer';
 
 const config = useRuntimeConfig();
 //aller a nuxt.config.ts
 const { data: myData } = await useFetch("nous-contacter", {
   baseURL: config.public.apiBase,
   headers: {
     Accept: "application/json",
     Authorization:
       "Basic " +
       Buffer.from("admin" + ":" + config.apiSecret).toString("base64"),
   },
 });
 console.log(myData.value);

function sendEmail() {

const mailaddress = document.getElementById("mail").value;
console.log("le mail tapé est" + mailaddress);
document.getElementById("msg").innerHTML = "Write your message";
 };





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
        text-transform: uppercase;
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