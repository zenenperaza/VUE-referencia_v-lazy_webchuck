<template>
<div> 
    <h1>Porcentage completado {{ percentage }}</h1>
</div>
</template>

<script lang="ts" >
import { defineComponent } from "vue"

export default defineComponent({
    data(){
        return {
            percentage:0
        }

    },

    methods: {
        recalculate() {
            this.percentage = 42 
        }
    },
    mounted(){
        this.percentage = 24
        }
})






</script>

<style scoped>

</style>