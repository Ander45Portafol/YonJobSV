<template>
  <div class="w-full">
    <div class="ms-4">
      <h5 class="font-bold text-2xl text-[#3459F4]">Experiencias</h5>
      <h6 class="text-[#45C567]">
        Revisa las empresas donde realizo las pasantías
      </h6>
    </div>
  </div>
</template>

<script setup>
import JobCard from "~/components/JobCard.vue";
import {
  MagnifyingGlassCircleIcon,
  MagnifyingGlassIcon,
} from "@heroicons/vue/20/solid";

definePageMeta({
  layout: "main",
});
</script>
<style scoped></style>
