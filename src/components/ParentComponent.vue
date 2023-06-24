<template>
<ChildComponent ref="percentageComponent"></ChildComponent>
<button v-on:click="banco">Add cuenta bancaria</button>
</template>

<script lang="ts">
import ChildComponent from './ChildComponent.vue';
import { defineComponent } from "vue";

export default defineComponent({
    components: {
        ChildComponent
    },
    methods: {
        banco(){
           this.$refs.percentageComponent.recalculate()
        }
    }
    
})


   
</script>

<style scoped>

</style>