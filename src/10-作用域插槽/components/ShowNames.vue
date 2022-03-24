<template>
  <div class="show-names">
    <template v-for="item in names">
      <slot :item="item"></slot>
    </template>
  </div>
</template>

<script>
export default {
  data() {
    return {
      names: ['kobe', 'james', 'even']
    }
  }
}
</script>

<style scoped></style>
