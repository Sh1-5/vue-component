<template>
  <div class="app">
    <ShowMessage class="message" message="Hello Vue" :info="info" />
    <MultiRootElement id="multi-root-element" />
  </div>
</template>

<script>
import ShowMessage from './components/ShowMessage.vue'
import MultiRootElement from './components/MultiRootElement.vue'

export default {
  data() {
    return {
      info: {
        name: 'kobe',
        age: 18
      }
    }
  },
  components: {
    ShowMessage,
    MultiRootElement
  }
}
</script>

<style scoped></style>
