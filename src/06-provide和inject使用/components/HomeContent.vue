<template>
  <div class="home-content">
    <ul>
      <li>{{ name }}</li>
      <li>{{ age }}</li>
      <li>{{ height }}</li>
      <!-- <li>{{ height.value }}</li> -->
    </ul>
  </div>
</template>

<script>
export default {
  inject: ['name', 'age', 'height']
}
</script>

<style scoped></style>
