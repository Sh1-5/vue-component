<template>
  <div class="app">
    <button
      v-for="item in tabs"
      :key="item"
      @click="itemClick(item)"
      :class="{ active: currentTab === item }"
    >
      {{ item }}
    </button>
    <keep-alive>
      <component :is="currentTab"></component>
    </keep-alive>
  </div>
</template>

<script>
import Home from './components/Home.vue'
import About from './components/About.vue'
import Category from './components/Category.vue'

export default {
  data() {
    return {
      tabs: ['home', 'about', 'category'],
      currentTab: 'home'
    }
  },
  components: {
    Home,
    About,
    Category
  },
  methods: {
    itemClick(item) {
      this.currentTab = item
    }
  }
}
</script>

<style scoped>
.active {
  color: red;
}
</style>
