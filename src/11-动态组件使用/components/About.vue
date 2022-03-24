<template>
  <div class="about">
    <h1>当前计数：{{ counter }}</h1>
    <button @click="increment">+1</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      counter: 0
    }
  },
  methods: {
    increment() {
      this.counter++
    }
  }
}
</script>

<style scoped></style>
