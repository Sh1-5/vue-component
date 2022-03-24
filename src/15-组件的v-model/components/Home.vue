<template>
  <div class="home">
    <ul>
      <li>{{ modelValue.name }}</li>
      <li>{{ modelValue.age }}</li>
      <li>{{ modelValue.height }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    modelValue: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped></style>
