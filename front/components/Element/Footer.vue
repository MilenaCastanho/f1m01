<template>
    <div class="conteiner">
        <div class="footer">
            <div class="footer_link">
                <ul>
                    <li><NuxtLink to="/">Logo</NuxtLink>
                        <img src="../assets/img/logo2.png" alt="Logo">
                    </li>
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/">Sobre</NuxtLink></li>
                    <li><NuxtLink to="/">Contato</NuxtLink></li>
                    <li><NuxtLink to="/">Login</NuxtLink></li>
                </ul>
            </div>
            <div class="footer_btn">
                <li class="btn play"><NuxtLink to="/">Play</NuxtLink></li>
                <li class="btn super"><NuxtLink to="/">Superlicense</NuxtLink></li>
            </div>
        </div>
    </div>  
</template>
<style scoped>
.footer {
    width: 100%;
    height: 100%;
    background-color: #000;
    display: flex;
    justify-content: space-between;
    align-items: center;
    box-shadow: 0px 0px 10px 0px #000;
}


</style>