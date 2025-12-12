<template>
  <div class="bg-[#E6EAEF] rounded-lg shadow-md p-6 w-full">
    <!-- Área de carga -->
    <div
      class="border-2 border-dashed border-[#3459F4] rounded-lg flex flex-col items-center justify-center p-8 cursor-pointer hover:bg-blue-50 transition"
      @click="triggerUpload"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="h-10 w-10 text-[#3459F4] mb-2"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 16v1a2 2 0 002 2h12a2 2 0 002-2v-1M12 12v6m0 0l-3-3m3 3l3-3M12 4v4m0 0l-3-3m3 3l3-3"
        />
      </svg>
      <p class="text-sm text-[#3459F4]">Subir CV</p>
      <input
        type="file"
        ref="fileInput"
        class="hidden"
        @change="handleFileUpload"
      />
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const fileInput = ref(null);

function triggerUpload() {
  fileInput.value.click();
}

function handleFileUpload(event) {
  const file = event.target.files[0];
  if (file) {
    console.log("Archivo seleccionado:", file.name);
  }
}
</script>
