<script setup lang="ts">
import { ref } from 'vue'
const active = ref(false)
const toggleNavigation = () => active.value = !active.value
</script>

<template>
  <nav class="fixed top-0 w-full left-0 bg-gray-800 text-white">
    <button @click="toggleNavigation">Click Me</button>
    {{active ? 'Hello' : 'Bye'}}
  </nav>
</template>