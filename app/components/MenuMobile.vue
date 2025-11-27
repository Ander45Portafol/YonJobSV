<template>
  <nav class="relative flex flex-1 flex-col">
    <ul role="list" class="flex flex-1 flex-col gap-y-7">
      <li>
        <ul role="list" class="-mx-2 space-y-1">
          <li>
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
              to="/cv_profesional"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-bold"
            >
              <NewspaperIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">CV profesional</span>
            </NuxtLink>
            <NuxtLink
              to="/experiencias"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-bold"
            >
              <DocumentTextIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">Experiencias</span>
            </NuxtLink>
          </li>
        </ul>
      </li>
      <li>
        <div class="text-xs/6 font-semibold text-gray-400">Pasantías</div>
        <ul role="list" class="-mx-2 mt-2 space-y-1">
          <li>
            <NuxtLink
              to="/oportunidades"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-bold"
            >
              <CheckBadgeIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">Oportunidades</span>
            </NuxtLink>
            <NuxtLink
              to="/conexiones"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-bold"
            >
              <LinkIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">Conexiones</span>
            </NuxtLink>
            <NuxtLink
              to="/recomendaciones"
              class="mt-2 bg-transparent text-[#D9EEF3] transform-gpu transition-transform duration-200 ease-in-out hover:scale-110 group flex gap-x-2 rounded-md p-3 text-sm/6 font-bold"
            >
              <HandThumbUpIcon class="size-6 shrink-0" aria-hidden="true" />
              <span class="">Recomendaciones</span>
            </NuxtLink>
          </li>
        </ul>
      </li>
      <li class="mt-auto">
        <a
          href="#"
          class="group-mx-2 flex gap-x-3 rounded-md p-2 text-sm/6 font-semibold text-gray-300 hover:bg-white/5 hover:text-white"
        >
          <Cog6ToothIcon
            class="size-6 shrink-0 text-gray-400 group-hover:text-white"
            aria-hidden="true"
          />
          Ajustes
        </a>
      </li>
    </ul>
  </nav>
</template>
<script setup>
import {
  HomeIcon,
  NewspaperIcon,
  DocumentTextIcon,
  CheckBadgeIcon,
  LinkIcon,
  HandThumbUpIcon,
  Cog6ToothIcon,
} from "@heroicons/vue/20/solid";
</script>
