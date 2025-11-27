<template>
  <!--Componente que muestra un resumen de las aplicaciones hechas. Se muestra en dashboard screen-->
  <div
    class="container flex flex-row items-center justify-between mx-auto sm:px-6 lg:px-6 bg-[#E6EAEF] rounded-xl p-3 m-3"
  >
    <!-- Sección izquierda (imagen y textos) -->
    <div class="flex items-center space-x-4">
      <img class="w-16 h-16 object-contain" :src="img" alt="icon" />
      <div>
        <h6 class="font-bold text-lg text-[#0E3266]">{{ name }}</h6>
        <p class="font-semibold text-base text-[#5A91FF]">{{ role }}</p>
      </div>
    </div>

    <!-- Botón al final -->
    <button
      type="button"
      class="flex items-center justify-center gap-x-1.5 rounded-md bg-[#5A91FF] px-3 py-2 text-sm text-white hover:bg-indigo-400 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-500"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="size-6"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M3.75 3.75v4.5m0-4.5h4.5m-4.5 0L9 9M3.75 20.25v-4.5m0 4.5h4.5m-4.5 0L9 15M20.25 3.75h-4.5m4.5 0v4.5m0-4.5L15 9m5.25 11.25h-4.5m4.5 0v-4.5m0 4.5L15 15"
        />
      </svg>
    </button>
  </div>
</template>

<script setup>
defineProps({
  img: {
    type: String,
    required: true,
  },
  name: {
    type: String,
    default: "Nombre",
  },
  role: {
    type: String,
    default: "Cargo",
  },
});
</script>
