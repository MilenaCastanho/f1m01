<template>
    <div class="conteiner">
        <div class="navbar">
            <div class="menu">
                    <NuxtLink to="/">
                        <img src="../assets/img/logo.png" alt="Logo">
                    </NuxtLink>                    
                    <NuxtLink to="/">F1</NuxtLink>
                    <NuxtLink to="/">News</NuxtLink>
                    <NuxtLink to="/">SocialMedia</NuxtLink>
                    <NuxtLink to="/">Fantasy</NuxtLink>
            </div>
            <div class="buttons">
               <NuxtLink class="btn play" to="/">Play</NuxtLink>
                <NuxtLink class="btn super" to="/login">Superlicense</NuxtLink>
            </div>
        </div>  
    </div>
</template>
<style scoped>
    .conteiner {
        width: 100%;
        height: 100%;
        background-color: #000;
    }
    .navbar {
        width: 100%;
        height:40px;
        background-color: #000;
        display: flex;
        justify-content: space-between;
        align-items: center;
        box-shadow: 0px 0px 10px 0px #000;
    }
    .menu {
        width: 100%;
        max-width: 400px;
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 20px;
    }
    .menu img {
        width: 100px;
        height: 100px;
    }
    .menu a {
        color: #c7c7c7;
        text-shadow: 0px 0px 10px #000;
        font-weight: bold;
        font-size: .80rem;
        text-decoration: none;
        margin: 0 15px;
        transition: 3ms;
    }
    .menu a:hover {
        color: #fff;
    }
    .menu a:active {
        color: #fdd800;
    }
    .buttons {
        display: flex;
        justify-content: space-between;
        align-items: center;        
    }
    .btn {
        width: 110px;
        height: 25px;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 2px;
        text-shadow: 0px 0px 10px #000;
        font-weight: bold;
        font-size: .80rem;
        text-decoration: none;
        margin: 0 15px;
        color: white;
    }
    .play {
        background-color: darkred;
        margin-right: 20px;
    }
    .play:hover, :active {
        background-color: red;
    }
    .super {
        background-color: darkgreen;
    }
    .super:hover, :active {
        background-color: green;
    }
</style>