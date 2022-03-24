<template>
  <div class="app">
    <Home v-model="info" />
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  data() {
    return {
      info: {
        name: 'kobe',
        age: 18,
        height: 1.8
      }
    }
  },
  components: {
    Home
  }
}
</script>

<style scoped></style>
