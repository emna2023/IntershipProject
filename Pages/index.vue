<template>
    <main class="main">

<div class="main__carroussel"> 
        <div class="main__carroussel__container" id="container">
             <img class="main__carroussel__container__img" alt="img1" src="../public/Media/image1.jpg" /> 
        </div>
        <img class="main__carroussel__buttonL" id="laft" alt="bt1" src="../public/Media/arrow_back_ios.png" />
        <img class="main__carroussel__buttonR" id="right" alt="bt2" src="../public/Media/arrow_forward_ios.png" />


        

</div>

        <div class="main__secondcontainer"> 
        <h2 class="main__secondcontainer__subtitle">Dernier épisode:</h2>
        <h1 class="main__secondcontainer__title">katana VS TRONCONNEUSE</h1>
        <ul>

        <li><div class="main__secondcontainer__imgcontainer">
            <img class="main__secondcontainer__imgcontainer__img" alt="img1" src="../public/Media/2Chainsaw-Man.jpg" />
        </div></li>
        <li>        <h2 class="main__secondcontainer__subtitle2">
                     Chapitres 35-36-37-38-40
                    </h2></li>

    </ul>

    </div>
    </main>
</template>
<script setup>

// document.body.onload=function(){
//     nbr=2;
//     container=document.getElementById("container");

//     for (i=1;i<=nbr;i++)
//     {
//         div=document.createElement("div");
//         div.className="img";
//         div.style.backgroundimage="url('/Media/image"+i+".jpg')";
//         container.appendChild(div);

//     }
//     g=document.getElementById("left");
//     //document.getElementById("right").onclick(function(),)
// }
</script>

<style lang="scss">
 .img{
            width: 100%;
            height: 400px;
            margin:0;
            display: inline-block;
           object-fit: cover;
        }

ul{
    display: grid;
    grid-template-columns: 70% 30%;
    list-style: none;
}

.main{
  //width: 100%;
  //height: 100%;
  margin-left: 0;
  margin-right: 0;
  margin-top: 0;

   &__carroussel{
    width:100%;
    height:400px;
    border: solid;
    overflow:hidden;
    position:relative;

    //pour fixer le cadre de la carroussel
    &__container{
    //display:flex;
    width:100%;
    height:400px;
    //position:relative;
    &__img{
            width: 100%;
            height: 400px;
            margin:0;
            display: inline-block;
           object-fit: cover;
        }

       
    }
    &__buttonL
    {
        position:absolute;
        width:70px;
        cursor: pointer;
        top:150px;
        left:0;
    }
    &__buttonR
    {
        position:absolute;
        width:70px;
        cursor: pointer;
        top:150px;
        right:0;
    }
}
        &__secondcontainer{
             margin-left:30px;
             margin-bottom: 250px;
             width:90%;
             height: 500px;
             overflow:visible;

            background-color: rgb(255, 196, 0);
            position:relative;
            &__subtitle{
                color:white;
                padding-left: 5px;
            }
            &__title{
              font-size: 4em;
            }
            &__imgcontainer{
                &__img{
                    position:absolue;
                    width:100%;
                    
                }
        }
    }
    
}
</style>