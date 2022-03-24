<template>
  <div class="app">
    <MySlotCpn>
      <i>Hello Vue</i>
      <div>Hello Vue</div>
    </MySlotCpn>
    <MySlotCpn>
      <strong>Hello Vue</strong>
      <span>Hello Vue</span>
    </MySlotCpn>
    <MySlotCpn>Hello Vue</MySlotCpn>
    <MySlotCpn />
  </div>
</template>

<script>
import MySlotCpn from './components/MySlotCpn.vue'

export default {
  components: {
    MySlotCpn
  }
}
</script>

<style scoped></style>
