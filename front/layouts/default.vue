<script lang="ts" setup></script>

<template>
  <div>
    <ElementNavbar />
    <section>
	    <slot />
    </section>
    <ElementFooter />
  </div>
</template>
<style scoped>
  section {
    min-height: 100vh;
  }
</style>
<style scoped>
  section {
    min-height: 100vh;
    background: linear-gradient(100deg, #000000 -60%, rgba(0,0,0,0) 50%, rgba(0,0,0,0.9) 120%) 0 / cover, 
    linear-gradient(180deg, #000000 -15%, rgba(0,0,0,0) 50%, #000000 130%) 0 / cover, 
    linear-gradient(#000000 1%, rgba(0,0,0,0.1), #000000 100%) 0 / 4px 4px, 
    radial-gradient(#000000 1%, rgba(0,0,0,0) 50%, #04032f 100%) 0 / 4px 4px, 
    url() #000000 0 / cover no-repeat;
  }
</style>