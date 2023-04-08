<template>
    <div >
       {{ name}}
    </div>
</template>

<script setup>
    const props = defineProps({
       name:{
        type:String
       }
    })
    console.log(props);
</script>

<style scoped>

</style>