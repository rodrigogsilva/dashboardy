<template lang="">
  <div>Counter {{ counterStore.count }}</div>
  <button
    type="button"
    class="rounded-full shadow border-transparent border-r-8 bg-purple-500 hover:bg-purple-600 active:bg-purple-700 focus:outline-none focus:ring focus:ring-purple-300 px-6 py-3 text-base font-medium text-white md:py-4 md:px-8 md:text-lg capitalize"
    @click="counterStore.increment"
  >
    increase
  </button>
</template>
<script setup lang="ts">
import { useCounterStore } from '@/stores/counter';

const counterStore = useCounterStore();
</script>
<style lang=""></style>
