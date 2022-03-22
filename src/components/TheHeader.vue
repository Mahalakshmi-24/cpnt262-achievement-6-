<template>
   <TheNavBar />
   <div class="flex flex-col"> 
  <h1 class="text-5xl">{{props.title}}</h1>
  
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