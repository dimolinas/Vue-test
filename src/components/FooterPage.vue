<template>
    <div class="Footer-container">
        <div class="logo"></div>
    </div>
</template>

<style scoped>

.Footer-container{
    height: 80px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    width: 100%;
    padding-right: 40px;
    background-color: white;
}

.logo{
    background-image: url("../assets/footer.png");
    width: 300px;
    height: 60px;
    background-position: 50% 50%;
    background-size: cover;
    background-repeat: no-repeat;
}

@media (max-width:700px) {
    .Footer-container{
        height: 40px;
    }

    .logo{
        width: 170px;
        height: 40px;
    }
    
}

</style>