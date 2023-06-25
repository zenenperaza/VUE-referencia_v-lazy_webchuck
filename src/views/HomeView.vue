<template>
<<<<<<< HEAD
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

export default defineComponent({
  name: 'HomeView',
  components: {
    HelloWorld,
  },
});
=======
<ParentComponent></ParentComponent>
</template>

<script lang="ts" setup>
import ParentComponent from '@/components/ParentComponent.vue';


>>>>>>> d0f003e398d4347eb66463b7b89dd47fbb72cb7b
</script>
