<template>
  <div class="w-full flex flex-col gap-4">
    <div class="ms-4">
      <h5 class="font-bold text-2xl text-[#3459F4]">Curriculum Vitae</h5>
    </div>
    <UploadCv />
    <div class="flex justify-end">
      <button
        type="button"
        class="rounded-full bg-[#0E3266] px-3.5 py-2 text-sm font-semibold text-white hover:bg-[#5A91FF] focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[#5A91FF]"
      >
        Crear cv
      </button>
      <button
        type="button"
        class="rounded-full ml-2 bg-[#0E3266] px-3.5 py-2 text-sm font-semibold text-white hover:bg-[#5A91FF] focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[#5A91FF]"
      >
        Analizar
      </button>
    </div>
    <div class="grid grid-cols-2">
      <ResultsTable />
      <div class="gap-4 ml-2">
        <div class="ms-4">
          <h5 class="font-bold text-lg text-[#3459F4]">Sugerencias</h5>
        </div>
        <div
          class="bg-white border border-[#5A91FF] rounded-md p-4 max-w-xl mx-auto mt-6"
        >
          <ul class="space-y-2">
            <li
              v-for="(item, index) in sugerencias"
              :key="index"
              class="flex items-start"
            >
              <span class="mt-1 mr-2 w-2 h-2 rounded-full bg-red-600"></span>
              <span class="text-sm text-[#5A91FF]">{{ item }}</span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import UploadCv from "~/components/UploadCv.vue";
import ResultsTable from "~/components/ResultsTable.vue";
definePageMeta({
  layout: "main",
});

const sugerencias = [
  "Detallar y mejorar habilidades blandas.",
  "Especificar qué tipo de habilidades técnicas posee.",
];
</script>
<style scoped></style>
