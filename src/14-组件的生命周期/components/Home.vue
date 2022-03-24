<template>
  <div class="home"></div>
</template>

<script>
export default {
  beforeCreate() {
    console.log('home beforeCreate')
  },
  created() {
    console.log('home created')
  },
  beforeMount() {
    console.log('home beforeMount')
  },
  mounted() {
    console.log('home mounted')
  },
  beforeUpdate() {
    console.log('home beforeUpdate')
  },
  updated() {
    console.log('home updated')
  },
  beforeUnmount() {
    console.log('home beforeUnmount')
  },
  unmounted() {
    console.log('home unmounted')
  },
  beforeDestroy() {
    console.log('home beforeDestroy')
  },
  destroyed() {
    console.log('home destroyed')
  }
}
</script>

<style scoped></style>
