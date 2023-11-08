<template>
  <div class="flex justify-center items-center h-screen">
    <div class="bg-gray-200 p-6 rounded-lg w-3/10">
      <h2 class="text-xl font-bold mb-4">Multiselect Dropdown</h2>
      <Homepage msg="Welcome to Your Vue.js App"/>
    </div>
  </div>
</template>

<script>
import Homepage from './components/HomePage.vue'

export default {
  name: 'App',
  components: {
    Homepage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
