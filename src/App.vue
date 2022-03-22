<template>

  <TheHeader :title="pageHeader"  />

  <TheFooter />

</template>

<script setup>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'

const pageHeader ='The New Page';

</script>

