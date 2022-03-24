<template>
  <div class="app">
    <Home />
    <About />
  </div>
</template>

<script>
import Home from './components/Home.vue'
import About from './components/About.vue'

export default {
  components: {
    Home,
    About
  }
}
</script>

<style scoped></style>
