<script setup>
import FooterPage from './FooterPage.vue';
defineProps({
    numberPage: Number
});

</script>

<template>
    
    <div class="header-container">
        <div class="footer-container">
            <FooterPage/>
        </div>
        <div class="nav-header">
            <h3>Curso: Emprendedor y Emprendimiento en El Salvador y La Región</h3>
        </div>
    </div>
    <div class="number-page">
        <div class="box-number-page">
            <h2>Página {{numberPage}} de 20</h2>
        </div>
    </div>
</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@600&display=swap');

.header-container{
    width: 100%;
    height: 10vh;
    display: flex;
    background-color: white;
}
.number-page{
    width: 100%;
    height: 40px;
    display: flex;
    justify-content: flex-end;
    background-color: white;
}
.footer-container{
    width: 30%;
    height: 100%;
}
.nav-header{
    width:70%;
    height: 100%;
    background-image: url("../assets/back.png");
    background-repeat: no-repeat;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    font-family: 'Rubik', sans-serif;
    color: white;
    
}
.box-number-page{
    width: 300px;
    height: 100%;
    border: 4px #7DBE43 solid ;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #006936;
    font-family: 'Rubik', sans-serif;
    font-size: small;
}

.box-number-page h2{
    color: #006936;
}

.nav-header h3{
    margin-right: 1.5rem;
}

@media (max-width:700px){
    .header-container{
        display: flex;
        flex-direction: column;
        height: max-content;
    }

    .footer-container{
        width: 100%;
        height: max-content;
        display: flex;
        justify-content: flex-end;
    }

    .nav-header{
        width: 100%;
        height: 7vh;
        display: flex;
        justify-content: flex-end;
    }

    .nav-header h3{
        width: 60%;
        font-size: 12px;
    }

    .number-page{
        height: 30px;
    }
    .box-number-page{
        width: 150px;
        height: 100%;
    }
}
</style>