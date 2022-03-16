<script setup>
import { ref,reactive } from 'vue';

import Header from './components/Header.vue';
import Main from './components/Main.vue';

const smth = ref("Some text");
</script>

<template>
  <img src="./assets/blobnew.png" alt="blob" class="headblob">
  <Header/>
  <Main/>
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

.headblob{
  position: absolute;
  z-index: -2;
  width: 800px;
  right: 0;
  top: 0;
  margin: 0;
}

</style>
