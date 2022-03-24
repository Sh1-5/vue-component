<template>
  <div class="about"></div>
</template>

<script>
import emitter from '../../utils/event-bus'

export default {
  created() {
    emitter.on('sendMessage', (info) => {
      console.log(info)
    })
  }
}
</script>

<style scoped></style>
