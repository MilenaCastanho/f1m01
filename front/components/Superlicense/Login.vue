<template>
  <div class="login">
    <div class="form">
      <h1 class="title">Login</h1>
      <NuxtLink  to="/register">
        <h3 class="subtitle">Not a member yet?</h3>
      </NuxtLink>
      <form @submit.prevent="submit">
        <div class="input">
          <input
            type="email"
            id="email"
            v-model="email"
            placeholder="Email"
          />
          <input
          type="password"
          id="password"
          v-model="password"
          placeholder="Password"
          />
        </div>
        <div class="checkbox">
          <input type="checkbox" v-model="checked">Keep me logged in
        </div>
       <button class="button" type="submit">Login</button>
      </form>
    </div>
  </div>
</template>
<style scoped>
.login {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
.form {
  width: 400px;
  height: 400px;
  background-color: linear-gradient(#070707, black, #030303)  ;
  border-radius: 5px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  padding: 40px;
}
.title {
  color: #fff;
  text-shadow: 0px 0px 5px rgb(4, 4, 4, 0.1);
  font-size: 2rem;
  margin-bottom: 10px;
}
.title :hover {
  color: #fff;
  text-shadow: 0px 0px 5px rgb(7, 7, 7);
}
.subtitle {
  text-align: right;
  font-size: 1rem;
  color: #fff;
  margin-bottom: 20px;
  text-decoration: none;
  border-bottom-style: none;
}
.subtitle :hover {
  color: #fff;
}
.input {
  display: flex;
  flex-direction: column;
  margin: 20px;
}
.input input {
  border: none;
  background-color: #070707;
  color: #fff;
  border: solid 1pd #fff;
  border-radius: 2px;
  background: #202020;
  padding: 10px;
  margin-bottom: 10px;
  font-size: 1.2rem;
  text-align: left;
  text-indent: 1.5rem;
  font-weight: bold;
  font-family: 'Play';
}
.input input:focus {
  outline: none;
}
.checkbox {
  display: flex;
  justify-content: center;
  align-items: left;
  margin: 20px;
}
.checkbox input {
  width: 20px;
  height: 20px;
  margin: 0 10px;
  align-items: left;
}
.checkbox label {
  color: #fff;
  font-size: 1rem;
}
.button {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 20px;
  padding: 10px;
  border: none;
  background-color: #070707;
  color: #fff;
  border: solid 1pd #fff;
  border-radius: 2px;
  background: #202020;
  padding: 10px;
  margin-bottom: 10px;
  font-size: 1.2rem;
  text-align: center;
  text-indent: 1.5rem;
  font-weight: bold;
  font-family: 'Play';
}
.button:focus {
  outline: none;
}
.button:hover {
  background-color: #fff;
  color: #070707;
}

/* old projects */

.modal-log-login {
  grid-area: b;
  padding: 20px;
  /*background: black;*/
  background: url("/assets/img/PIT-BOARD13.png?h=7edfcf2eb0f3cfef9ee98209560e9677") center/cover no-repeat black;
  height: 400px;
  box-shadow: 1px 1px 5px 5px #020202;
  width: 270px;
  border: solid 1px #555555;
  display: grid;
  border-radius: 10px;
  justify-items: center;
  justify-content: center;
  align-content: start;
  grid-gap: 30px;
  transition: 1s;
}


</style>

