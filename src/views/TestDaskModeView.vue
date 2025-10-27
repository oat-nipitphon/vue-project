<template>
  <div :class="isDark ? 'dark' : ''" class="min-h-screen bg-white dark:bg-gray-900 dark:text-white transition-all">
    <div class="p-10">
      <h1 class="text-3xl font-bold mb-4">🌞 Light / 🌙 Dark Mode</h1>
      <button @click="isDark = !isDark" class="px-4 py-2 bg-blue-600 text-white rounded-lg hover:bg-blue-700">
        Toggle Mode
      </button>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
const isDark = ref(false)
</script>
