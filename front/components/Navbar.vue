<template>
    <img :src="logo" alt="logo" />
    <nav>
      <ul>
        <li v-for="item in navbar" :key="item.id">{{ item.label }}</li>
      </ul>
    </nav>
    <button @click="btn1">{{ btn1.name }}</button>
 </template>
  
  <script setup lang="ts">
  import { defineComponent, defineProps } from 'vue';
  
     defineComponent({
    props: {
    logo:{
        type: String,
        name: String,
        required: true,
        default: () => '',
      },  
    navbar: {
        type: Array,
        required: true,
        default: () => [],
      },
    btn1: {
        type: Object,
        required: true,
        default: () => {},
      },      
    }
  });
  </script>
  