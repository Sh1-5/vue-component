<template>
  <div class="counter-operation">
    <button @click="increment">+1</button>
    <button @click="decrement">-1</button>
    <div>
      <input type="text" v-model.number="value" />
      <button @click="incrementN">+N</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      value: 10
    }
  },
  emits: ['increment', 'decrement', 'incrementN'],
  methods: {
    increment() {
      this.$emit('increment')
    },
    decrement() {
      this.$emit('decrement')
    },
    incrementN() {
      this.$emit('incrementN', this.value)
    }
  }
}
</script>

<style scoped></style>
