<template>
    <div>
        <button>
            <slot></slot>
        </button>

    </div>
</template>

<script setup lang="ts">
//Using Nuxt js and typescript, create a button component?



</script>

<style scoped>
.button {
  text-decoration: none;
  text-transform: uppercase;
  font-size: 0.65rem;
  font-weight: bold;
  max-width: 150px;
  min-width: 90px;
  width: 100%;
  height: 25px;
  display: grid;
  text-shadow: 0px 1px 5px black;
  border: solid 1px;
  border-radius: 3px;
  align-items: center;
  white-space: nowrap;
  justify-content: center;
  transition: 0.2s;
}

</style>