<template>
  <div class="mb-5">
    <BoxApp/>
  </div>
  <div class="mb-5">
    <TitleApp/>
  </div>
  <div class="d-flex justify-content-center">
   <ButtonList/>
  </div>
</template>

<script setup>
  import ButtonList from './components/ButtonList/ButtonList.vue';
  import BoxApp from './components/Box/BoxApp.vue';
  import TitleApp from './components/Title/TitleApp.vue';
</script>

<style  scoped>

</style>