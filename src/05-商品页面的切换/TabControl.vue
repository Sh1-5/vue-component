<template>
  <div class="tab-control">
    <div
      class="title"
      :class="{ active: currentIndex === index }"
      v-for="(title, index) in titles"
      :key="title"
      @click="titleClick(index)"
    >
      <span>{{ title }}</span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentIndex: 0
    }
  },
  props: {
    titles: {
      type: Array,
      required: true
    }
  },
  emits: ['titleClick'],
  methods: {
    titleClick(index) {
      this.currentIndex = index
      this.$emit('titleClick', index)
    }
  }
}
</script>

<style scoped>
.tab-control {
  display: flex;
}

.title {
  flex: 1;
  text-align: center;
  cursor: pointer;
}

.title span {
  padding: 5px 5px;
}

.active {
  color: red;
}

.active span {
  border-bottom: 5px solid red;
}
</style>
