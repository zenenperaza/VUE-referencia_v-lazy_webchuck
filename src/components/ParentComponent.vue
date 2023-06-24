<template>
<ChildComponent ref="percentageComponent"></ChildComponent>
<button v-on:click="banco">Add cuenta bancaria</button>
</template>

<script lang="ts" setup>
import ChildComponent from './ChildComponent.vue';
import { ref } from "vue";

const percentageComponent = ref(null)

const banco = () => {
    percentageComponent.value.recalculate()
}
   
</script>

<style scoped>

</style>