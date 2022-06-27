<template>
  <div class="my-input">
    <input type="text" :value="modelValue" @input="inputChange" />
    <input type="text" v-model="value" />
  </div>
</template>

<script>
export default {
  props: ['modelValue'],
  emits: ['update:modelValue'],
  methods: {
    inputChange(e) {
      this.$emit('update:modelValue', e.target.value)
    }
  },
  computed: {
    value: {
      get() {
        return this.modelValue
      },
      set(value) {
        this.$emit('update:modelValue', value)
      }
    }
  }
}
</script>

<style scoped></style>
