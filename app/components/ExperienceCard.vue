<template>
  <div
    class="w-full rounded-lg border-2 border-[#5A91FF] bg-white p-6 shadow-sm"
  >
    <div class="mb-4 flex items-center justify-between">
      <div>
        <h2 class="text-lg font-bold text-[#051E51]">{{ namee }}</h2>
        <p class="text-sm font-semibold text-[#5A91FF]">{{ role }}</p>
      </div>
      <div class="flex items-center space-x-1">
        <StarIcon
          v-for="i in 5"
          :key="i"
          :class="['h-5 w-5', i <= grade ? 'text-[#BDDF22]' : 'text-gray-300']"
          aria-hidden="true"
        />
      </div>
    </div>

    <div class="mb-2 text-sm text-[#5A91FF] font-semibold flex flex-row gap-4">
      <p>
        <span class="font-semibold text-[#051E51]">Fecha inicio:</span>
        {{ startDate }}
      </p>
      <p>
        <span class="font-semibold text-[#051E51]">Fecha finalización:</span>
        {{ endDate }}
      </p>
    </div>

    <p class="mt-4 text-sm font-semibold text-[#5A91FF] leading-relaxed">
      <span class="text-[#051E51]"> Comentarios: </span>
      {{ comments }}
    </p>
  </div>
</template>

<script setup>
defineProps({
  namee: String,
  role: String,
  startDate: String,
  endDate: String,
  comments: String,
  grade: String,
});
import { StarIcon } from "@heroicons/vue/20/solid";
</script>
