<template>
  <div class="show-message">
    <h1 :class="$attrs.class">{{ message }}</h1>
    <ul>
      <li>{{ info.name }}</li>
      <li>{{ info.age }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  // props: ['message']
  props: {
    message: String,
    info: {
      type: Object,
      required: true
    }
  },
  inheritAttrs: false
}
</script>

<style scoped></style>
