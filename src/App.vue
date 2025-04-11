<script setup lang="ts">
import CounterVue from './components/counter.vue'
</script>

<template>
  <CounterVue />
  <p class="text-green-500 text-8xl text-center justify-center">Hello World</p>
  <nav class="flex justify-center gap-4 my-5">
    <RouterLink class="bg-blue-400 text-green-900 p-5" to="/">Kembali Pulang</RouterLink>
    <RouterLink class="bg-blue-400 text-green-900 p-5" to="/counter">Tambah Counter</RouterLink>
  </nav>
  <main>
    <RouterView />
  </main>
</template>
