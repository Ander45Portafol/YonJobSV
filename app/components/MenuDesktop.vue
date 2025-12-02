<template>
  <nav class="flex flex-1 flex-col">
    <ul role="list" class="flex flex-1 flex-col gap-y-7">
      <li>
        <ul role="list" class="-mx-2 space-y-1">
          <li class="mt-2">
            <NuxtLink
              to="/dashboard"
              class="bg-[#D9EEF3] text-[#5A91FF] hover:bg-white/5 hover:text-white', 'group flex gap-x-3 rounded-md p-3 text-sm/6 font-bold"
            >
              <HomeIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">Dashboard</span>
            </NuxtLink>
          </li>
        </ul>
      </li>
      <li>
        <div class="text-xs/6 font-semibold text-gray-400">Datos</div>
        <ul role="list" class="-mx-2 mt-2 space-y-1">
          <li>
            <NuxtLink
              to="/"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-normal"
            >
              <NewspaperIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">CV profesional</span>
            </NuxtLink>

            <NuxtLink
              to="/"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-normal"
            >
              <BriefcaseIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">Aplicaciones</span>
            </NuxtLink>

            <NuxtLink
              to="/"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-normal"
            >
              <DocumentTextIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">Portafolio</span>
            </NuxtLink>
          </li>
        </ul>
      </li>
      <li>
        <div class="text-xs/6 font-semibold text-gray-400">Pasantías</div>
        <ul role="list" class="-mx-2 mt-2 space-y-1">
          <li>
            <NuxtLink
              to="/"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-normal"
            >
              <GlobeAsiaAustraliaIcon
                class="size-6 shrink-0"
                aria-hidden="true"
              />
              <span class="">Oportunidades</span>
            </NuxtLink>
            <NuxtLink
              to="/"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-normal"
            >
              <ChatBubbleOvalLeftEllipsisIcon
                class="size-6 shrink-0"
                aria-hidden="true"
              />
              <span class="">Mensajes</span>
            </NuxtLink>
            <NuxtLink
              to="/"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-normal"
            >
              <ChartBarSquareIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">Experiencias</span>
            </NuxtLink>
          </li>
        </ul>
      </li>
      <li class="mt-auto">
        <NuxtLink
          to="/"
          class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-normal"
        >
          <Cog6ToothIcon class="size-6 shrink-0" aria-hidden="true" />
          <span class="">Ajustes</span>
        </NuxtLink>
      </li>
    </ul>
  </nav>
</template>
<script setup>
import {
  HomeIcon,
  NewspaperIcon,
  DocumentTextIcon,
  ChatBubbleOvalLeftEllipsisIcon,
  ChartBarSquareIcon,
  Cog6ToothIcon,
  BriefcaseIcon,
  GlobeAsiaAustraliaIcon,
} from "@heroicons/vue/20/solid";
</script>
