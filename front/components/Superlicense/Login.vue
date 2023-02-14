<template>
  <div class="login">
    <div class="form">
      <h1 class="title">Login</h1>
      <NuxtLink class="subtitle" to="/register">
        Not a member yet?
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
  background-color: #f5f5f5;
}
.form {
  width: 400px;
  height: 400px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  padding: 20px;
}
.title {
  text-align: center;
  font-size: 2rem;
  font-weight: 500;
  margin-bottom: 10px;
}
.subtitle {
  text-align: center;
  font-size: 1rem;
  font-weight: 500;
  margin-bottom: 10px;
}
.input {
  display: flex;
  flex-direction: column;
  margin-bottom: 20px;
}
.input input {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  outline: none;
  margin-bottom: 10px;
}
.checkbox {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}
.checkbox input {
  margin-right: 10px;
}
.button {
  padding: 10px;
  border: none;
  border-radius: 5px;
  background-color: #000;
  color: #fff;
  font-size: 1rem;
  font-weight: 500;
  cursor: pointer;
}
</style>

