<template>
  
    <header class="text-center py-10">
      <h2 class=" text-4xl">{{props.title}}</h2>
    </header>

    <slot name="contentInfo"></slot>

</template>

<script setup>
import {defineProps} from 'vue';

const props = defineProps({
  title: {
    type: String
  }
});



</script>