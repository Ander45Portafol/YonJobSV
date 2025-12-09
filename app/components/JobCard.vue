<template>
  <div class="bg-[#E6EAEF] text-white rounded-lg shadow-md p-6 w-full max-w-md">
    <div class="flex items-center justify-between mb-2">
      <h2 class="text-lg font-bold text-[#051E51]">{{ company }}</h2>
      <span class="text-sm text-gray-400">{{ date }}</span>
    </div>
    <h3 class="text-indigo-400 text-md font-medium mb-2">{{ title }}</h3>
    <p class="text-sm text-[#051E51] line-clamp-3">{{ description }}</p>
  </div>
</template>

<script setup>
defineProps({
  company: String,
  date: String,
  title: String,
  description: String,
});
</script>

<style scoped>
.line-clamp-3 {
  display: -webkit-box;
  -webkit-box-orient: vertical;
  overflow: hidden;
}
</style>
