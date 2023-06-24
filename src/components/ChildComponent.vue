<template>
<div> 
    <h1>Porcentage completado {{ percentage }}</h1>
</div>
</template>

<script lang="ts" setup>
import { onMounted, ref, defineExpose } from "vue";  

const percentage = ref(0)

onMounted(() => {
    percentage.value = 24
})

const recalculate = ( ) => {
    percentage.value = 42
}

defineExpose({recalculate})

</script>

<style scoped>

</style>