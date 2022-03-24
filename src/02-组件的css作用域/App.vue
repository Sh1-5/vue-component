<template>
  <div class="app">
    <h1>App</h1>
    <About />
  </div>
</template>

<script>
import About from './components/About.vue'

export default {
  components: {
    About
  }
}
</script>

<style scoped>
h1 {
  color: red;
}
</style>
