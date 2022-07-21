<script setup>
import HeaderPage from './HeaderPage.vue';
defineProps({
    numberPage: Number
});

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
            <HeaderPage numberPage="1"></HeaderPage>
            <div class="main">
                <div class="person"></div>
                <div class="text-container">
                    <h1>Ideas de cierre</h1>
                    <h2>El ecosistema emprendedor y los emprendimientos dinámicos</h2>
                    <h2>Haz click en las personas </h2>
                </div>
            </div>
            <div class="svg-container">
                    
                        <svg width="758" height="413" viewBox="0 0 200.554 109.273" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="http://www.w3.org/2000/svg">
                        <g transform="translate(-494.892 -140.66)">
                            <ellipse cx="391.743" cy="50.835" rx="42.575" ry="16.726" fill="none"/>
                            <ellipse cx="321.937" cy="79.778" rx="7.096" ry="39.667" fill="none"/>
                            <ellipse cx="262.385" cy="52.642" rx="28.723" ry="22.088" fill="none"/>
                            <image width="200.554" height="109.273" preserveAspectRatio="none" xlink:href="../assets/diapositiva-17.png" x="494.892" y="140.661"/>
                            <g transform="translate(-11.82 -27.291)">
                            <ellipse cx="525.913" cy="190.034" rx="6.555" ry="6.62" fill="#7cbe43" stroke="#7cbe43" stroke-width=".265"/>
                            <text xml:space="preserve" style="line-height:1.25" x="545.622" y="184.793" transform="scale(.96018 1.04147)" font-weight="400" font-size="6.528" font-family="sans-serif" fill="#fff" stroke-width=".163"><tspan x="545.622" y="184.793">1</tspan></text>
                            </g>
                            <g transform="translate(56.927 8.588)">
                            <ellipse cx="543.654" cy="190.724" rx="6.555" ry="6.62" fill="#7cbe43" stroke="#7cbe43" stroke-width=".265"/>
                            <text xml:space="preserve" style="line-height:1.25" x="564.18" y="185.139" transform="scale(.96018 1.04147)" font-weight="400" font-size="6.528" font-family="sans-serif" fill="#fff" stroke-width=".163"><tspan x="564.18" y="185.139">2</tspan></text>
                            </g>
                            <g transform="translate(9.053 -39.802)">
                            <ellipse cx="559.539" cy="189.747" rx="6.555" ry="6.62" fill="#7cbe43" stroke="#7cbe43" stroke-width=".265"/>
                            <text xml:space="preserve" style="line-height:1.25" x="580.642" y="184.517" transform="scale(.96018 1.04147)" font-weight="400" font-size="6.528" font-family="sans-serif" fill="#fff" stroke-width=".163"><tspan x="580.642" y="184.517">3</tspan></text>
                            </g>
                            <g transform="translate(73.198 24.274)">
                            <ellipse cx="462.364" cy="203.891" rx="6.555" ry="6.62" fill="#7cbe43" stroke="#7cbe43" stroke-width=".265"/>
                            <text xml:space="preserve" style="line-height:1.25" x="479.437" y="198.098" transform="scale(.96018 1.04147)" font-weight="400" font-size="6.528" font-family="sans-serif" fill="#fff" stroke-width=".163"><tspan x="479.437" y="198.098">4</tspan></text>
                            </g>
                        </g>
                    </svg>
            </div>
        </div>
    </div>
</template>

<style scoped>

    .svg-container{
        display: flex;
        width: 100%;
        height: max-content;
        justify-content: center;
        background-color: white;
        margin-bottom: 40px ;
    }

    .general{
        width: 100%;
        height: 100vh;
        display: flex;
    }
    .menu-burguer{
        width: 4%;
        height: 100%;
        background-color:#C2C3C9;
    }
    .page-one-container{
        width: auto;
        width: 96%;
        height: max-content;
        display: flex;
        flex-direction: column;
        background-color:white;
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
        margin-bottom: 2rem;

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