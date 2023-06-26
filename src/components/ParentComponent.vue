<template>
<div> 
    <img v-lazy="{ src: lazyOptions.src, lifecycle: lazyOptions.lifecycle, delay: lazyOptions.delay }" lazy="loading" style="max-width: 100%; height: auto;">
</div>
</template>

<script lang="ts" setup>
import { ref, VNode } from "vue";

const lazyOptions = ref({
    src: 'https://picsum.photos/2400/1800',
    delay: 500,
    lifecycle: {
        loading: (ele:VNode) => {
            console.log('cargando imagen', ele);
            
        },
        error: (ele:VNode) => {
            console.log('error en la carga', ele);
            
        },
        loaded: (ele:VNode) => {
            console.log('imagen cargada', ele) ;
            
        }
    }
})
   
</script>


<style scoped>

img[lazy=loading]{
    background-color: yellow;
    width: 500px;
}

</style>