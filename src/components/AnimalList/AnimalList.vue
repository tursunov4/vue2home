<template>
     <div class="box-title">
        <div class="box-animal" v-for="(item , index) in arr" :key="index">
            <h3>{{ item.name }}</h3>
            <h4>{{ item.first }}</h4>
            <h5>{{ item.massa }}</h5>
            <h5>{{ item.type }}</h5>
            <button>More</button>
           </div>
     </div>
</template>

<script setup>
   const props = defineProps({
    arr : {
        type : Array
    }
   })
   console.log(props);
</script>

<style  scoped>
 .box-title{
    gap: 40px;
    display: flex;
    align-items: center;
   justify-content: center;
 }
 .box-animal{
    width: 320px;
    padding: 20px;
    border: 2px solid;
 }
</style>