<script>
export default {
  data() {
    return {
        name: '',
        surname: '',
        email: '',
        password: ''
      }
  },
  methods: {
    async submit() {
      await fetch('http://localhost:8000/api/register', {
        method: 'POST',
        headers: {'Content-Type': 'application/json'},
        body: JSON.stringify(
          name: this.name,
          surname: this.surname,
          email: this.email,
          password: this.password,    
        )
      });
    }
  }
}


</script>
<template>
  <div class="register">
    <form @submit.prevent="submit">
      <h1 class="title">Register</h1>
      <NuxtLink class="subtitle" to="/login">Already a member?</NuxtLink>
        <div class="input">
          <input
            type="text"
            id="name"
            v-model="name"
            placeholder="Name"
          />
          <input
            type="text"
            id="surname"
            v-model="surname"
            placeholder="Surname"
          />
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
        <button class="button" type="submit">Register</button>
      </form>
    </div>

</template>
<style scoped>
.register {
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
  justify-content: center;
  align-items: center;
}
.input > input {
  width: 100%;
  margin: 10px 0;
  padding: 10px;
  outline: none;
  border: none;
  background-color: #f5f5f5;
  border-radius: 10px;
  font-size: 1rem;
}
.button {
  width: 100%;
  margin: 10px 0;
  padding: 10px;
  outline: none;
  border: none;
  background-color: #f5f5f5;
  border-radius: 10px;
  font-size: 1rem;
}
</style>