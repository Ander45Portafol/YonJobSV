<template>
  <div class="w-full">
    <div class="ms-4">
      <h5 class="font-bold text-2xl text-[#3459F4]">Experiencias</h5>
      <h6 class="text-[#45C567]">
        Revisa las empresas donde realizo las pasantías
      </h6>
    </div>
    <div class="w-full mt-4">
      <ExperienceCard
        namee="Ricaldone"
        role="programador"
        startDate="20/12/2025"
        endDate="07/01/2026"
        comments="Fugiat ipsum ipsum deserunt culpa aute sint do nostrud anim incididunt cillum culpa consequat. Excepteur qui ipsum aliquip consequat sint. Sit id mollit nulla mollit nostrud in ea officia proident. Irure nostrud pariatur mollit ad adipisicing reprehenderit deserunt qui eu."
        grade="4"
      />
    </div>
  </div>
</template>

<script setup>
import ExperienceCard from "~/components/ExperienceCard.vue";

definePageMeta({
  layout: "main",
});
</script>
<style scoped></style>
