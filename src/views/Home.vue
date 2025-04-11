<script setup lang="ts">
import { storeToRefs } from 'pinia'
import { useCounterStore } from '@/stores/counter'
const { count } = storeToRefs(useCounterStore())
</script>

<template>
  <p class="text-green-500 text-2xl">Counter Ngab {{ count }}</p>
</template>
