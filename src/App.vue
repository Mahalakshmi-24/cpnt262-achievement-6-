<template>

  <TheHeader :title="pageHeader"  />
  
  
  <TheArticle :title="articleTitle" class="px-5">
    <template #articleInfo>
      <p class="text-lg px-4">
        Welcome to Studio, A premiere studio rental location for photographers, videographers, and creatives. Please scroll down to look through all the features of the studio.
      </p>
    </template>
  </TheArticle>

  <TheContent :title="contentTitle" class="px-5">
    <template #contentInfo>
      <p class="text-lg px-4">
        A limited selection of draping, furniture and props are available for your use in all studios.</p>

      <p class="text-lg px-4"> We are always changing the props  to keep the studio fresh and current, some of our most popular props are listed below. </p>
       <section class="flex flex-col bg-gray-200  py-4">
      <ul class="text-center">
        <li class="py-3 " v-for="product in sets" :key="product.id">{{product}}</li>
      </ul>  
       </section>
    </template>
  </TheContent>


  <TheFooter />

</template>

<script setup>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
import TheArticle from './components/TheArticle.vue'
import TheContent from './components/TheContent.vue'

const pageHeader ='Studio';
const articleTitle ='FEATURES OF STUDIO A';
const contentTitle ='Props & Drops';

const sets = ['Vintage suitcases ', 'Baby props', 'Childrens furniture ', 'Faux fur pieces', 'Fabric draping'];


</script>

