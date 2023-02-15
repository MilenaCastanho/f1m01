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

/* old project */
footer {
  grid-area: footer;
  display: grid;
  justify-items: center;
  grid-template-areas: "nav" "log" "info" "socialMedia" "disc" "copy";
  background: black;
  box-shadow: 0px 0px 2px 2px black;
}

footer div {
  display: grid;
  grid-auto-flow: column;
  justify-content: center;
}

footer div {
  display: grid;
  grid-auto-flow: column;
  justify-content: center;
  padding: 0 10px;
  width: 100px;
}



footer p {
  color: #ddd;
  transition: 0.3s;
}
footer h3 {
  font-weight: bold;
  color: #555555;
  text-shadow: 1px 1px 3px black;
}

footer h3:hover {
  color: #ddd;
}


footer p {
  display: grid;
  max-width: 50%;
  /*grid-area: a;*/
  max-width: 70%;
  font-size: 0.7rem;
  padding: 15px 10px;
  color: #555555;
  font-weight: bold;
  transition: 0.3s;
  letter-spacing: 1px;
  text-align: center;
}

@media (min-width: 540px) {
  footer p {
    /*grid-area: a;*/
    max-width: 550px;
    font-size: 0.7rem;
    padding: 15px 10px;
    color: #555555;
    font-weight: 400;
    transition: 0.3s;
    letter-spacing: 1px;
    justify-items: center;
  }
}

footer p:hover {
  color: #ddd;
  transition: 0.3s;
}

footer a:hover {
  color: #ddd;
}

footer div img {
  height: 100px;
}

footer img {
  height: 75px;
}

@media (min-width: 320px) {
  footer img {
    grid-area: log;
    height: 100px;
  }
}




</style>