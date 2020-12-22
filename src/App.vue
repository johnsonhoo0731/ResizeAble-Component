<template>
  <div class="draggable-container" 
      ref="parentRef">
    <resize-able 
      parentRef="parentRef"
     >
      <button class="btn">button</button>
    </resize-able>
  </div>
</template>

<script>
import { ref } from "vue"
import ResizeAble from './components/ResizeAble.vue'
export default {
  name: 'App',
  components: {
    ResizeAble,
  },
}
</script>

<style scoped>
.draggable-container {
  width: 600px;
  height: 600px;
  border: 1px solid #aaa;
  margin: 0 auto;
  position: relative;
  box-sizing: border-box;
}
.btn {
  width: 100px;
  height: 50px;
  border: lightblue;
  background: lightblue;
  border-radius: 8px;
}
.img {
  width: 100px;
  height: 100px;
}
</style>