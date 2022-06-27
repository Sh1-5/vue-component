<template>
  <h2 :id="$attrs.id">MuliRootElement</h2>
  <h2>MuliRootElement</h2>
  <h2>MuliRootElement</h2>
</template>

<script>
export default {
  props: {
    name: String
  },
  mounted() {
    console.log(this.name)
  }
}
</script>

<style scoped></style>
