<template>
  <header>
    <Logo />
    <nav v-for="item in menuLink" :key="item.id">
       <NuxtLink :to="item.url">{{ item.name }}</NuxtLink>
    </nav>
  </header>
</template>

<script lang="ts" setup>

const logoUrl = ref( "@assets/img/logo/f1masterCom.png")

const menuLink = ref(
  [
    {
      id: 1,
      name: 'Home',
      url: '/',
    },
    {
      id: 2,
      name: 'About',
      url: '/about',
    },
    {
      id: 3,
      name: 'Contact',
      url: '/contact',
    },
  ]
)

const btn1 = ref(
  {
    name: 'Login',
    url: '/login',
  }
)
</script>

<style scoped>
  section {
    min-height: 100vh;
    background: linear-gradient(100deg, #000000 -60%, rgba(0,0,0,0) 50%, rgba(0,0,0,0.9) 120%) 0 / cover, 
    linear-gradient(180deg, #000000 -15%, rgba(0,0,0,0) 50%, #000000 130%) 0 / cover, 
    linear-gradient(#000000 1%, rgba(0,0,0,0.1), #000000 100%) 0 / 4px 4px, 
    radial-gradient(#000000 1%, rgba(0,0,0,0) 50%, #04032f 100%) 0 / 4px 4px, 
    url("../assets/img/driver.png") #000000 0 / cover no-repeat;
  }
</style>