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
footer a {
  color: grey;
  width: auto;
  letter-spacing: 1px;
  font-size: 0.68rem;
  font-weight: bold;
  padding: 5px 11px;
  display: flex;
  text-decoration: none;
  text-transform: capitalize;
  /*border: solid 0.9px black;*/
  white-space: nowrap;
  text-shadow: 0px 0px 5px #040404;
  background: #040404;
  justify-content: space-around;
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

footer img {
  height: 75px;
}

@media (min-width: 320px) {
  footer img {
    grid-area: log;
    height: 100px;
  }
}

footer {
  grid-area: footer;
  display: grid;
  justify-items: center;
  grid-template-areas: "nav" "log" "info" "disc" "copy";
  background: black;
  box-shadow: 0px 0px 2px 2px black;
}

footer div {
  display: grid;
  grid-auto-flow: column;
  justify-content: center;
}

footer h5 {
  color: grey;
  font-weight: bold;
}

footer h5:hover {
  color: white;
}

</style>