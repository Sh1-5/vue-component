<template>
  <div class="app">
    <NavBar>
      <template v-slot:left>
        <button>button</button>
      </template>
      <template v-slot:center>
        <span>span</span>
      </template>
      <template v-slot:right>
        <i>i</i>
      </template>
    </NavBar>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'

export default {
  components: {
    NavBar
  }
}
</script>

<style scoped></style>
