<template>
  <div class="app">
    <h1>{{ message }}</h1>
    <button @click="foo">foo</button>
    <Home />
  </div>
</template>

<script>
import mixin from './mixins/demo-mixin'
import Home from './components/Home.vue'

export default {
  mixins: [mixin],
  components: {
    Home
  }
}
</script>

<style scoped></style>
