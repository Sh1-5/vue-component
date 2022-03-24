<template>
  <div class="app">
    <h1>About</h1>
    <Home />
    <Suspense>
      <template #default>
        <AsyncAbout />
      </template>
      <template #fallback>
        <Loading />
      </template>
    </Suspense>
  </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'
import Home from './components/Home.vue'
import Loading from './components/Loading.vue'
const AsyncAbout = defineAsyncComponent(() =>
  import('./components/AsyncAbout.vue')
)
// const AsyncAbout = defineAsyncComponent({
//   loader: import('./components/AsyncAbout.vue'),
//   loadingComponent: Loading, // 占位组件，在未加载时显示的组件
//   delay: 2000, // 在显示loadingComponent之前等待多长时间
//   onError: function (err, retry, fail, attempts) {} // err：错误信息；retry：函数，调用retry尝试重新加载；fila：函数，指示加载程序退出；attempts：尝试次数
// })

export default {
  components: {
    Home,
    AsyncAbout,
    Loading
  }
}
</script>

<style scoped></style>
