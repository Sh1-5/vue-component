<template>
  <div class="app">
    <TabControl :titles="titles" @titleClick="titleClick" />
    <h1>{{ contents[currentIndex] }}</h1>
  </div>
</template>

<script>
import TabControl from './TabControl.vue'

export default {
  data() {
    return {
      titles: ['衣服', '鞋子', '裤子'],
      currentIndex: 0,
      contents: ['衣服页面', '鞋子页面', '裤子页面']
    }
  },
  components: {
    TabControl
  },
  methods: {
    titleClick(index) {
      this.currentIndex = index
    }
  }
}
</script>

<style scoped></style>
