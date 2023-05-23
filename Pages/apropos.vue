<template>
<main class="main">
<h1 class="main__title">A PROPOS</h1>
<div class="main__imgContainer">

        </div>

<h3 class="main__subTitle">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam eu tellus sed est fermentum iaculis. Fusce consequat odio eu fermentum scelerisque. Duis blandit diam quis ante luctus posuere. Mauris rutrum in urna ut placerat. Cras vitae sollicitudin mi. In nec sapien faucibus, gravida nunc facilisis, posuere metus. Pellentesque aliquam fermentum libero cursus cursus. Proin id porta velit. Integer et tellus consequat, imperdiet nibh id, auctor ex. Vestibulum porttitor ligula non pretium semper. Sed laoreet tempor erat, sit amet viverra diam malesuada nec. Suspendisse hendrerit, leo eu interdum tincidunt, felis massa dictum massa, quis ultrices ligula massa non nunc. In eleifend enim non rutrum volutpat. Donec mattis vel nisl vitae aliquam.

Aliquam ut tortor suscipit, mattis lorem at, pharetra dui. Ut semper diam augue, at sodales mi aliquam sit amet. Curabitur faucibus leo velit, non consectetur orci posuere et. Maecenas orci quam, ultricies sed mi non, tincidunt mollis felis. Suspendisse ac ex pharetra, suscipit tortor eget, consequat lectus. Sed elementum fermentum mi a bibendum. Suspendisse facilisis vel tellus eu mollis.
</h3>


</main>
</template>
<script lang="ts" setup>
</script>
<style scoped lang="scss">


.main{
    margin-right: 0;
    margin-left: 0;
    &__title{
        size: 60px;
        text-align: left;
        padding-left:30px;

        font-family: Georgia, 'Times New Roman', Times, serif;
        
    }
    &__imgContainer{
        background-image: url("/Media/4screenshot.jpg") ;
        background-attachment: fixed; /* Fixe l'image pendant le scroll */
        background-size: cover; /* L'image prendra 100% de l'espace, quitte à la crop */
        background-position: center; /* Centre la position de l'image */
        background-repeat: no-repeat; /* Empêche l'image de se répéter en fonction de la taille d'écran */
        height: 800px; /* On fixe une grande hauteur pour voir plus facilement le scroll */
        
         }
        &__subTitle{
            padding-left: 40px;
            padding-right: 30px;
        }
    }
</style>