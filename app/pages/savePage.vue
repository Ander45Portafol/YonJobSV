<template>
  <div class="w-full">
    <div class="ms-4">
      <h5 class="font-bold text-2xl text-[#3459F4]">Guardados</h5>
      <h6 class="text-[#45C567]">
        Revisa la lista de oportunidades que te interesan
      </h6>
    </div>
    <h6 class="ms-4 font-semibold text-[#000000] mt-4">Ordenar por:</h6>
    <div class="flex flex-row me-6 space-y-4">
      <!-- Dropdown Fecha -->
      <div class="ms-4 flex flex-col max-w-xs mr-4">
        <h6 class="mb-1 text-[#3459F4]">Fecha</h6>
        <el-select
          id="select-fecha"
          name="selected-fecha"
          class="w-full bg-[#E6EAEF] rounded-lg"
        >
          <button
            type="button"
            class="flex w-full items-center justify-between px-3 py-2 text-[#3459F4]"
          >
            <el-selectedcontent class="pr-6"
              >Seleccionar una opción</el-selectedcontent
            >
            <svg
              viewBox="0 0 16 16"
              fill="none"
              stroke="#3459F4"
              stroke-width="2"
              class="size-4"
            >
              <path d="M4 6l4 4 4-4" />
            </svg>
          </button>
          <!-- Opciones -->
          <el-options
            popover
            anchor="bottom start"
            class="mt-1 bg-white rounded-md shadow-md w-(--button-width) py-1"
          >
            <el-option
              value="1"
              class="px-3 py-2 text-gray-700 hover:bg-gray-100"
            >
              2026
            </el-option>
            <el-option
              value="2"
              class="px-3 py-2 text-gray-700 hover:bg-gray-100"
            >
              2025
            </el-option>
            <el-option
              value="3"
              class="px-3 py-2 text-gray-700 hover:bg-gray-100"
            >
              2024
            </el-option>
          </el-options>
        </el-select>
      </div>
      <!-- Dropdown Puesto -->
      <div class="flex flex-col max-w-xs">
        <h6 class="mb-1 text-[#3459F4]">Puesto</h6>
        <el-select
          id="select-puesto"
          name="selected-puesto"
          class="w-full bg-[#E6EAEF] rounded-lg"
        >
          <button
            type="button"
            class="flex w-full items-center justify-between px-3 py-2 text-[#3459F4]"
          >
            <el-selectedcontent class="pr-6"
              >Seleccionar una opción</el-selectedcontent
            >
            <svg
              viewBox="0 0 16 16"
              fill="none"
              stroke="#3459F4"
              stroke-width="2"
              class="size-4"
            >
              <path d="M4 6l4 4 4-4" />
            </svg>
          </button>
          <!-- Opciones -->
          <el-options
            popover
            anchor="bottom start"
            class="mt-1 bg-white rounded-md shadow-md w-(--button-width) py-1"
          >
            <el-option
              value="1"
              class="px-3 py-2 text-gray-700 hover:bg-gray-100"
            >
              San Salvador
            </el-option>
            <el-option
              value="2"
              class="px-3 py-2 text-gray-700 hover:bg-gray-100"
            >
              Santa Ana
            </el-option>
            <el-option
              value="3"
              class="px-3 py-2 text-gray-700 hover:bg-gray-100"
            >
              Apopa
            </el-option>
          </el-options>
        </el-select>
      </div>
    </div>
    <div class="w-full flex flex row ms-4">
      <JobCard
        image="./facebook.jpg"
        company="Facebook"
        date="20/11/2025"
        title="Analista de datos"
        description="Culpa consequat. Excepteur qui ipsum aliquip consequat sint. Sit id mollit nulla mollit nostrud in ea officia proident. Irure nostrud pariatur mollit ad adipisicing reprehenderit deserunt qui eu..."
      />
    </div>
  </div>
</template>

<script setup>
import JobCard from "~/components/JobCard.vue";
definePageMeta({
  layout: "main",
});
</script>
<style scoped></style>
