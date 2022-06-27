<template>
  <div class="app">
    <h2>App</h2>
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
h2 {
  color: red;
}
</style>
