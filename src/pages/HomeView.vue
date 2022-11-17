<style lang="SCSS" scoped></style>

<script setup>
// @ is an alias to /src
import JobAplllicationProcedure from '@/components/HomePage/JobAplllicationProcedure.vue'
import WelcomePageComponent from '@/components/HomePage/WelcomePageComponent.vue'
import Cat from '@/components/HomePage/categoriesComponent.vue'
</script>

<template>
  <div class="home">
    <WelcomePageComponent />
    <JobAplllicationProcedure />
    <Cat />
  </div>
</template>
