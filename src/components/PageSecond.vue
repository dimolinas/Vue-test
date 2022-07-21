<script setup>
import HeaderPage from './HeaderPage.vue';
</script>


<template>
    <div class="general">
        <div class="menu-burguer">
             <input id="toggler" type="checkbox" class="toggler">
                <a id="toggler" href="#" class="nav">
                    <div class="one"></div>
                    <div class="two"></div>
                    <div class="three"></div>
                    <div class="menu-container-general">
                        <div class="container-links">
                            <a href="historia.html">Inicio</a>                            
                        </div>
                        <div class="container-logo">
                            <div class="pencil"></div>
                            <div class="book"></div>
                        </div>
                    </div>
                </a>
        </div>
        <div class="page-one-container">
            <HeaderPage></HeaderPage>
            <div class="main">
                <div class="person"></div>
                <div class="text-container">
                    
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .general{
        width: 100%;
        height: 100vh;
        display: flex;
    }
    .menu-burguer{
        width: 4%;
        height: 100vh;
        background-color:#C2C3C9;
    }
    .page-one-container{
        width: auto;
        width: 96%;
        height: 100vh;
        display: flex;
        flex-direction: column;
        background-color: antiquewhite;
    }
    .person{
        width: 180px;
        height: 180px;
        border-radius: 100%;
        background-image: url("../assets/person.png");
        background-repeat: no-repeat;
        background-size: contain;
        background-position: 50% 50%;
        margin-left: 6rem;
        margin-right: 6rem;
        margin-bottom: 1rem;

    }
    .main{
        display: flex;
        width: 100%;
        height: max-content;
        background-color: white;
    }

    .nav div{
    height: 5px;
    background-color: #006936;   
    margin: 5px 0;
    border-radius: 24px;
    transition: .3s;
    
}


.pencil{
    width: 50px;
    height: 50px;
    background-image: url("../assets/pensil.png");
    background-repeat: no-repeat;
    background-position: 50% 50%;
    background-size: cover;
    margin: 30px;
}

.book{
    width: 50px;
    height: 50px;
    margin: 30px;
    background-image: url("../assets/book.svg");
    background-repeat: no-repeat;
    background-position: 50% 50%;
    background-size: cover;
}

.nav{
    display: block;
    z-index: 3;
    left: 5%;
    top:3%;
    /* border:2px solid white; */
    margin:0 ;
    width: 50px;
    transition:  all 0.4s ease;
}

.toggler{
    position: absolute;
    left: 5%;
    top: 3%;
    z-index: 4;
    width: 50px;
    height: 50px;
    opacity: 0;
}

.one{
    width: 70%;
    z-index: 1;
}

.two{
    width: 50%;
}

.three{
    width: 40%;;
}

.toggler:hover + .nav div{
    width: 100%;
}


/* .toggler:checked + .nav .three{
    display: none;
}
 */
 .menu-container-general{
    position: fixed;
    left: -100%;
    top: 0%;
    width: 25%;
    height: 100%;
    z-index: 2;
    background-color:#C2C3C9;
    display: flex;
    flex-direction: column;
    opacity: 0.85;
    justify-content: center;
    align-items: center;
    transition: cubic-bezier(.46,.03,.52,.96) 0.4s;
}

.container-links{
    width: 100%;
    height: 50%;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    background-color: transparent;
}

.container-logo{
    width: 100%;
    height: 50%;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    background-color: transparent;
}

.menu-container-general a{
    width: max-content;
    font-size: 4rem;
    font-family: "Homework";
    text-decoration: none;
    color: #fff;
    transition: ease 0.4s;
}

.menu-container-general a:hover{
    color: #262b2c;
    font-size: 5rem;
}

.toggler:checked + .nav .two{
    transform: rotate(135deg); 
    width: 70%;
}

.toggler:checked + .nav .three{
    width: 70%;
    -webkit-transform: translateY(-10px) rotate(-135deg);
}


.toggler:checked + .nav .one{
    display: none;
}
 
.toggler:checked ~ .menu-container-general{
    left: 0%;
    top: 0%;
}

</style>