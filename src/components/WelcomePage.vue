<script setup>
import FooterPage from './FooterPage.vue';

</script>

<template>
    <div class="welcome-page-container">
        <div class="text-start-container">
            <div class="text-box-container">
                <div class="center-container">
                    <h2 class="welcome-text animate__bounceInLeft">Bienvenido al curso</h2>
                    <h2 class="bold animate__bounceInLeft">Emprendedores y Emprendimiento <br> En el salvador y la región </h2>
                </div>
            </div>
            <div class="start">
                <div class="button-start">
                    <h1>Iniciar</h1>
                </div>
                
            </div>

        </div>
        <div class="triangle"></div>
        <FooterPage></FooterPage>
    </div>

</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@600&display=swap');

.welcome-page-container{
    width: 100%;
    height: 85vh;
}
.text-start-container{
    width: 100%;
    display: flex;
    height: 90%;
    background-color: bisque;
}
.text-box-container{
    width: 50%;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    font-size: 20px;
    color: white;
    background-color: #006936;
    justify-content: center;
}

.bold{
    font-family: 'Rubik', sans-serif;
    color: white;

}

.start{
    width: 50%;
    display: flex;
    align-items: center;
    background-color: #006936;
    justify-content: center;
}

.button-start{
    width: 153px;
    height: 153px;
    background-color: transparent;
    background-image: url("../assets/botonInicio.93dec749.png");
    background-position: 50% 50%;
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    color: white;
    font-size: 15px;
    font-family: 'Rubik', sans-serif;
    justify-content: center;
    align-items: center;
}

.button-start:hover{
    width: 170px;
    height: 170px;
    animation-duration: 0.75s;
    font-size: 18px;
}

.center-container{
    display: flex;
    background-color: transparent;
    align-items: center;
    flex-direction: column;
    justify-content: flex-start;
}
.center-container h2{
    width: 100%;
}

.welcome-text{
    color: #7DBE43;
}

.triangle{
    width: 100%;
    height: 15vh;
    background-image: url("../assets/rectangule.svg");
    background-position: 50% 50%;
    background-size: cover;
    background-repeat: no-repeat;
}

@media (max-width: 1024px){

}

@media ( max-width: 700px) {

    .welcome-page-container{
        height: 70vh;
    }
    .text-start-container{
        width: 100%;
        height: 90%;
        flex-direction: column;
        align-items: center;
    }

    .center-container{
        align-items: center;
        justify-content: center;
    }

    .text-box-container{
        width: 100%;
        height: 50%;
        align-items: center;
        font-size: small;
    }

    .start{
        width: 100%;
        height: 50%;
    }
}


</style>


