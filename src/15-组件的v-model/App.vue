<template>
  <div class="app">
    <MyInput v-model="value" />
    <MyInput :modelValue="value" @update:modelValue="updateValue" />
    <button @click="handleClick">查看value</button>
  </div>
</template>

<script>
import MyInput from './components/MyInput.vue'

export default {
  data() {
    return {
      value: ''
    }
  },
  components: {
    MyInput
  },
  methods: {
    handleClick() {
      console.log(this.value)
    },
    updateValue(value) {
      this.value = value
    }
  }
}
</script>

<style scoped></style>
