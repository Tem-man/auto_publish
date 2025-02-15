<script setup>
import { ref } from 'vue'
const count = ref(0)
const handleCount = (a) => {
  console.log("dsdll", a);
  if (a === 1) {
    count.value += 1;
  } else {
    count.value -= 1;
  }
}
</script>

<template>

  <div class="card">
    <button type="button" @click="handleCount(1)">+1</button>
    <button type="button" @click="handleCount(2)">-1</button>
    <div class="count">{{ count }}</div>
  </div>


</template>

<style scoped>
.count {
  margin-top: 10px;
  padding: 5px 0;
  border-radius: 6px;
  background-color: aliceblue;
  font-size: 16px;
  font-weight: 500;
}

.read-the-docs {
  color: #888;
}
</style>
