<script setup lang="ts">
import { useCounterStore } from '@/stores/counter'
import { storeToRefs } from 'pinia'

const store = useCounterStore()
const { count } = storeToRefs(store)

const increment = () => {
  store.increment()
}
</script>

<template>
  <button @click="increment" class="bg-red-100 text-red-800 px-4 py-3 cursor-pointer">
    Tambah
  </button>
  <p class="text-red-800">{{ count }}</p>
</template>
