<template>
  <div class="home">
    <h2>Home</h2>
    <button @click="getParent">获取parent</button>
    <button @click="getRoot">获取root</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: 'Home'
    }
  },
  methods: {
    logMessage() {
      console.log('logMessage')
    },
    getParent() {
      console.log(this.$parent)
    },
    getRoot() {
      console.log(this.$root)
    }
  }
}
</script>

<style scoped></style>
