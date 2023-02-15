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
               <NuxtLink class="btn play" to="/">
                <ElementButton
                    text="Play"
                    color="#fff"
                    background="#070707"
                    border="1px solid #fff"
                    radius="2px"
                    padding="10px"
                    margin="0 10px"
                    size="1.2rem"
                    weight="bold"
                    family="Play"
                
                />

            </NuxtLink>
                <NuxtLink class="btn super" to="/superlicense">
                <ElementButton
                	onclick="handleSuperlicense()"
                    text="Superlicense"
                    color="#fff"
                    background="#070707"
                    border="1px solid #fff"
                    radius="2px"
                    padding="10px"
                    margin="0 10px"
                    size="1.2rem"
                    weight="bold"
                    family="Play"
                />
                </NuxtLink>
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

    /* old project */
    @media (min-width: 540px) {
  Header {
    display: grid;
    grid-area: header;
    grid-template-areas: "log nav . btn1 btn2";
    height: 40px;
    width: 100%;
    align-content: center;
    justify-content: space-evenly;
    background: black;
    box-shadow: 0px 0px 2px 2px rgba(6,6,6,0.6);
  }
}

@media (max-width: 539px) {
  header {
    background: black;
    display: grid;
    grid-template-areas: "log btn1 btn2" "nav nav nav";
    padding: 10px;
    grid-gap: 5px;
    height: 80px;
    align-content: center;
    justify-content: space-around;
    box-shadow: 0px 0px 10px 10px rgba(6,6,6,0.6);
  }
}

    @media (min-width: 600px) {
  .logo {
    /*display: none;*/
    grid-area: log;
    height: 15px;
    width: auto;
    padding: 0 5px;
    cursor: pointer;
  }
}

.logo {
  grid-area: log;
  height: 15px;
  width: auto;
  padding: 0 5px;
  cursor: pointer;
}

.playToEarn a {
    text-decoration: none;
    text-transform: uppercase;
    font-size: 0.65rem;
    font-weight: bold;
    max-width: 200px;
    width: 100%;
    height: 25px;
    display: grid;
    border: inset 1px;
    align-items: center;
    white-space: nowrap;
    justify-content: center;
    transition: 0.2s;
}

nav a {
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
    /*background: #040404;*/
    justify-content: space-around;
    transition: 0.25s;
}

nav a:active {
    color: #fdd800;
    /*border: solid 0.8px rgba(253,216,0,0);*/
    border-radius: 3px;
    transition: 0.2s;
    /*background: rgba(253,216,0,0.05);*/
}

nav a:hover {
    color: #fdd800;
    /*border: solid 0.8px rgba(253,216,0,0);*/
    border-radius: 3px;
    transition: 0.3s;
}

nav {
    display: flex;
    align-self: center;
    justify-content: space-between;
    grid-area: nav;
    grid-template-columns: repeat(4, 60px);
}

.button.superlicense:hover {
    color: white;
    background: radial-gradient(green, darkgreen);
    border: inset 1px darkgreen;
}

.button.superlicense:active {
  color: white;
  background: radial-gradient(green, darkgreen);
  border: inset 1px darkgreen;
}

.button.playToEarn:hover {
  color: white;
  background: radial-gradient(red, darkred);
  border: inset 1px darkred;
}

.button.playToEarn:active {
  color: white;
  background: radial-gradient(red, darkred);
  border: inset 1px darkred;
}

.btn.playToEarn:hover {
  color: white;
  background: radial-gradient(red, darkred);
  border: inset 1px darkred;
}

.btn.playToEarn:active {
  color: white;
  background: radial-gradient(red, darkred);
  border: inset 1px darkred;
}

.button.superlicense {
  grid-area: btn2;
  color: green;
  border: solid 1px green;
  border-radius: 3px;
  /*min-width: 100px;*/
}

.button.playToEarn {
  grid-area: btn1;
  color: red;
  border: solid 1px red;
  border-radius: 3px;
  /*min-width: 100px;*/
}

</style>
