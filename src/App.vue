<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router';
import Header from '@/components/Header.vue';
</script>

<template>
  <div id="app">
    <Header />
    <RouterView />
  </div>
</template>

<style scoped>
#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.header {
  width: 100%;
}
</style>
