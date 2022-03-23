<template>
  
   <div class="flex flex-row py-8 px-10 bg-blue-300"> 
    <img src="../assets/logo.png" alt="logo-image" class="w-11 h-11 " >
  <h1 class=" text-4xl">{{props.title}}</h1>
   <TheNavBar />
  </div>
  
  
  
</template>

<script setup>
import {defineProps} from 'vue';

import TheNavBar from './TheNavBar.vue'

const props = defineProps({
  title: {
    type: String
  }
});



</script>