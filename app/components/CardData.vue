<template>
  <!--Componente que muestra -->
  <div
    class="flex items-center gap-4 p-5 rounded-2xl text-white m-2 shadow-sm transition-transform duration-200 hover:scale-[1.02]"
    :style="{ backgroundColor: color?.startsWith('#') ? color : `#${color}` }"
  >
    <!-- Ícono -->
    <div class="flex items-center justify-center bg-white/20 rounded-xl p-3">
      <slot name="icon"></slot>
    </div>

    <!-- Texto -->
    <div class="flex flex-col leading-tight">
      <p class="text-4xl font-extrabold -mb-1">{{ camp }}</p>
      <p class="text-lg font-light">{{ title }}</p>
    </div>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  camp: Number,
  color: String,
});
</script>
