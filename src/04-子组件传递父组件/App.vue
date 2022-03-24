<template>
  <div class="app">
    <h1>当前计数: {{ counter }}</h1>
    <CounterOperation
      @increment="increment"
      @decrement="decrement"
      @incrementN="incrementN"
    />
  </div>
</template>

<script>
import CounterOperation from './compoents/CounterOperation.vue'

export default {
  data() {
    return {
      counter: 0
    }
  },
  components: {
    CounterOperation
  },
  methods: {
    increment() {
      this.counter++
    },
    decrement() {
      this.counter--
    },
    incrementN(N) {
      this.counter += N
    }
  }
}
</script>

<style scoped></style>
