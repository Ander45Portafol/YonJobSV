<template>
  <div class="bg-[#E6EAEF] text-white rounded-lg shadow-md p-6 w-full max-w-md">
    <!-- Encabezado con imagen, nombre, título y fecha -->
    <div class="flex items-start justify-between mb-4">
      <!-- Imagen + texto -->
      <div class="flex items-center gap-4">
        <img
          :src="image"
          alt="Logo empresa"
          class="w-12 h-12 rounded-full object-cover bg-white"
        />
        <div>
          <h2 class="text-lg font-bold text-[#051E51]">{{ company }}</h2>
          <h3 class="text-indigo-400 text-md font-medium">{{ title }}</h3>
        </div>
      </div>

      <!-- Fecha -->
      <span class="text-sm text-[#45C567] whitespace-nowrap">{{ date }}</span>
    </div>

    <!-- Descripción -->
    <p class="text-sm text-[#051E51] line-clamp-3">{{ description }}</p>
  </div>
</template>

<script setup>
defineProps({
  company: String,
  date: String,
  title: String,
  description: String,
  image: String,
});
</script>

<style scoped>
.line-clamp-3 {
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
}
</style>
