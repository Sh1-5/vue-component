<template>
  <div class="app">
    <h2>当前计数：{{ counter }}</h2>
    <button @click="increment">+1</button>
    <Home />
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  data() {
    return {
      counter: 0
    }
  },
  components: {
    Home
  },
  beforeCreate() {
    console.log('beforeCreate')
  },
  created() {
    console.log('created')
  },
  beforeMount() {
    console.log('beforeMount')
  },
  mounted() {
    console.log('mounted')
  },
  beforeUpdate() {
    console.log('beforeUpdate')
  },
  updated() {
    console.log('updated')
  },
  beforeUnmount() {
    console.log('beforeUnmount')
  },
  unmounted() {
    console.log('unmounted')
  },
  beforeDestroy() {
    console.log('beforeDestroy')
  },
  destroyed() {
    console.log('destroyed')
  },
  methods: {
    increment() {
      this.counter++
    }
  }
}
</script>

<style scoped></style>
