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
