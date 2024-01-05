<script setup lang="ts">
const count = ref(0)
const countUp = () => {
  count.value++
}
const countDown = () => {
  if (count.value > 0) {
    count.value--
  }
}
</script>

<template>
  <p class="text-2xl text-center w-full">{{ count }}</p>
  <div class="flex gap-x-4">
    <button class="btn" @click="countUp">たす</button>
    <button class="btn" @click="countDown">ひく</button>
  </div>
</template>