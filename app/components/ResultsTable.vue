<template>
  <div class="gap-4 px-3 sm:px-6 lg:px-6">
    <div class="sm:flex sm:items-center">
      <div class="sm:flex-auto"></div>
      <div class="sm:mt-0 sm:ml-16 sm:flex-none"></div>
    </div>
    <div class="">
      <h5 class="font-bold text-lg text-[#3459F4]">Resultados</h5>
    </div>
    <div class="flow-root">
      <div class="-mx-4 -my-2 overflow-x-auto sm:-mx-6 lg:-mx-8">
        <div class="inline-block min-w-full py-2 align-middle">
          <table class="relative min-w-full divide-y divide-[#6A9AFD]">
            <thead>
              <tr>
                <th
                  scope="col"
                  class="py-3.5 pr-3 pl-4 text-left text-sm font-semibold text-[#051E51] sm:pl-6 lg:pl-8"
                >
                  N
                </th>
                <th
                  scope="col"
                  class="px-2 py-3.5 text-left text-sm font-semibold text-[#051E51]"
                >
                  Titulo
                </th>
                <th
                  scope="col"
                  class="px-3 py-3.5 text-left text-sm font-semibold text-[#051E51]"
                >
                  Descripción
                </th>
                <th
                  scope="col"
                  class="px-3 py-3.5 text-left text-sm font-semibold text-[#051E51]"
                >
                  Porcentaje de error
                </th>
              </tr>
            </thead>
            <tbody class="divide-y divide-[#6A9AFD] bg-white">
              <tr v-for="person in people" :key="person.email">
                <td
                  class="py-4 pr-3 pl-4 text-sm font-medium whitespace-nowrap text-black sm:pl-6 lg:pl-8"
                >
                  {{ person.n }}
                </td>
                <td class="px-3 py-4 text-sm whitespace-nowrap text-gray-400">
                  {{ person.title }}
                </td>
                <td class="px-3 py-4 text-sm whitespace-pre-line text-gray-400">
                  {{ person.descripcion }}
                </td>
                <td class="px-3 py-4 text-sm whitespace-nowrap text-gray-400">
                  {{ person.porcentaje }}
                </td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const people = [
  {
    n: "1",
    title: "Habilidades blandas",
    descripcion: "La sección de habilidades blandas, no es clara.",
    porcentaje: "76%",
  },
  {
    n: "2",
    title: "Habilidades técnicas",
    descripcion: "La sección de habilidades blandas, no es clara.",
    porcentaje: "20%",
  },
];
</script>
