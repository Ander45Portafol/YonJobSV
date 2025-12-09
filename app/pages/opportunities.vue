<template>
  <!--Aqui va la parte del encabezado-->

  <div class="w-full flex flex-col gap-4">
    <div class="ms-4">
      <h5 class="font-bold text-2xl text-[#3459F4]">Oportunidades</h5>
      <h6>Pasantías</h6>
    </div>
    <div class="flex flex-row">
      <label for="email-address" class="sr-only">Email address</label>
      <input
        id="buscar-pasantia"
        type="pasantia"
        name="pasantia"
        required
        placeholder="Buscar pasantía"
        autocomplete="email"
        class="min-w-0 flex-auto rounded-md bg-[#E6EAEF] px-3.5 py-2 text-base text-[#5A91FF] outline-1 -outline-offset-1 outline-[#E6EAEF] placeholder:text-[#5A91FF] focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-500 sm:text-sm/6"
      />
      <el-select
        id="select"
        name="selected"
        value="Ciudad"
        class="m-2 block bg-[#E6EAEF] rounded-lg"
      >
        <button
          type="button"
          class="flex w-full items-center justify-between px-3 py-2 text-[#3459F4]"
        >
          <el-selectedcontent class="col-start-1 row-start-1 pr-6"
            >Ciudad</el-selectedcontent
          >

          <!-- Flecha -->
          <svg
            viewBox="0 0 16 16"
            fill="none"
            stroke="#3459F4"
            stroke-width="2"
            aria-hidden="true"
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
      <el-select
        id="select"
        name="selected"
        value="Categorías"
        class="m-2 block bg-[#E6EAEF] rounded-lg"
      >
        <button
          type="button"
          class="flex w-full items-center justify-between px-3 py-2 text-[#3459F4]"
        >
          <el-selectedcontent class="col-start-1 row-start-1 pr-6"
            >Categorias</el-selectedcontent
          >

          <!-- Flecha -->
          <svg
            viewBox="0 0 16 16"
            fill="none"
            stroke="#3459F4"
            stroke-width="2"
            aria-hidden="true"
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
            Categoria 1
          </el-option>
          <el-option
            value="2"
            class="px-3 py-2 text-gray-700 hover:bg-gray-100"
          >
            Categori 2
          </el-option>
          <el-option
            value="3"
            class="px-3 py-2 text-gray-700 hover:bg-gray-100"
          >
            Categoria 3
          </el-option>
        </el-options>
      </el-select>
    </div>
    <div class="w-full flex flex row">
      <JobCard
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
