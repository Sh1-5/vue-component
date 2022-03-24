<template>
  <div class="home">
    <button @click="btnClick">按钮点击</button>
  </div>
</template>

<script>
import emitter from '../../utils/event-bus'

export default {
  methods: {
    btnClick() {
      emitter.emit('sendMessage', { name: 'kobe', age: 18 })
    }
  }
}
</script>

<style scoped></style>
