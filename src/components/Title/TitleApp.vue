<template>
    <div>
      <h1 class="text-center mb-5">
        Animals 
      </h1>
      <AnimalList :arr="arr"/>
    </div>
</template>

<script setup>
   import { ref } from 'vue';
   import AnimalList from '../AnimalList/AnimalList.vue';
   const arr = ref([
     {
        name:'Lion',
        first:'Panthero leo',
        massa : '140kg',
        type : 'meat'
     },
     {
        name:'Gorrilla',
        first:'Gorilla beringei',
        massa : '205kg',
        type : 'plants , incents'
     },
     {
        name:'Zebra',
        first:'Equos quaga',
        massa : '322kg',
        type : 'plants'
     },
   ])
</script>

<style scoped>

</style>