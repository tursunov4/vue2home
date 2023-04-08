<template>
     <div >
        <div>
            <button @click="num =1">Invose 1</button>
            <button @click="num=2">Invose 2</button>
            <button @click="num=3">Invose 3</button>
            <button @click="num=4">Invose 4</button>
         </div>
         <div v-if="num == 1" class="wrapper-button">
           <ButtonTitle :name="in1"/>
         </div>
         <div v-else-if="num == 2" class="wrapper-button">
           <ButtonTitle :name="in2"/>
         </div>
         <div v-else-if="num == 3" class="wrapper-button">
           <ButtonTitle :name="in3"/>
         </div>
         <div v-else-if="num == 4" class="wrapper-button">
           <ButtonTitle :name="in4"/>
         </div>
     </div>
</template>

<script setup>
 import { ref } from 'vue';
 import ButtonTitle from '../ButtonTitle/ButtonTitle.vue';
 const num = ref(1)
 const in1 = ref('Invoce 1')
 const in2 = ref('Invoce 2')
 const in3 = ref('Invoce 3')
 const in4 = ref('Invoce 4')
</script>

<style scoped>
.wrapper-button{
    width: 400px;
    height: 400px;
    border: 1px solid;
}
</style>