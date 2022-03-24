<template>
  <div class="app">
    <!-- <ChildCpn>
      <span>{{ title }}</span>
    </ChildCpn> -->
    <ShowNames>
      <template v-slot="slotProps">
        <strong>{{ slotProps.item }}</strong>
      </template>
    </ShowNames>
  </div>
</template>

<script>
import ChildCpn from './components/ChildCpn.vue'
import ShowNames from './components/ShowNames.vue'

export default {
  components: {
    ChildCpn,
    ShowNames
  }
}
</script>

<style scoped></style>
