<template>
  <div class="app">
    <Home />
  </div>
</template>

<script>
import { computed } from 'vue'
import Home from './components/Home.vue'

export default {
  data() {
    return {
      height: 1.8
    }
  },
  components: {
    Home
  },
  // provide: {
  //   name: 'kobe',
  //   age: 18
  // }
  provide() {
    return {
      name: 'kobe',
      age: 18,
      // height: this.height
      // 使用computed包裹，height是响应式的
      height: computed(() => this.height)
    }
  }
}
</script>

<style scoped></style>
