<script setup>
import { ref,reactive } from 'vue';

import Header from './components/Header.vue';

const smth = ref("Some text");
</script>

<template>
  <Header/>
</template>

<style>
#app {
  font-family: 'Montserrat', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  max-width: 100vw;
  margin: 40px;
}


</style>
