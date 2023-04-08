<template>
    <div class="box">
     <HeaderApp style="width: 360px; background-color: yellow; text-align: center; padding: 5px; margin: 10px auto; " :name="name"  />
     <div class="d-flex gap-4">
        <HeaderApp :name="nav" style="width: 40px; height: 200px; background-color: green; text-align: center; " />
        <div>
            <HeaderApp style="width: 300px; height: 50px; margin-bottom: 20px; margin-top: 7px;   background-color: aqua; text-align: center;" :name="figure" />
            <HeaderApp style="width: 300px; height: 50px; margin-bottom: 20px; background-color: aqua; text-align: center;" :name="figure" />
            <HeaderApp style="width: 300px; height: 50px; margin-bottom: 20px; background-color: aqua; text-align: center;" :name="figure" />
        </div>
     </div>
     <HeaderApp style="width: 360px; background-color: yellow; text-align: center; padding: 5px; margin: 5px auto; " :name="footer" />
    </div>
</template>

<script setup>
import { ref } from 'vue';
import HeaderApp from '../Header/HeaderApp.vue';
const name = ref('Header') 
const nav = ref('nav')
const figure = ref('figure')
const footer = ref('footer')
</script>

<style  scoped>

</style>