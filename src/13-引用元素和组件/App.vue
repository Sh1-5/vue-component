<template>
  <div class="app">
    <h2 id="title" ref="title">Hello Vue</h2>
    <button @click="btnClick">获取h1元素</button>
    <button @click="getCpn">获取Home组件</button>
    <hr />
    <Home ref="home" />
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  components: {
    Home
  },
  methods: {
    btnClick() {
      console.log(this.$refs.title)
    },
    getCpn() {
      console.log(this.$refs.home.message)
      this.$refs.home.logMessage()
    }
  }
}
</script>

<style scoped></style>
