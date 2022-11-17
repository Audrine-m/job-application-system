<template>
  <div class="container track-application">
    <nav aria-label="breadcrumb">
      <ol class="breadcrumb">
        <li class="breadcrumb-item"><a href="#">track-application</a></li>
        <li class="breadcrumb-item active" aria-current="page">job</li>
      </ol>
    </nav>
    <cards />
    <cards />
    <cards />
    <cards />
  </div>
</template>

<script setup>
import cards from '@/components/track-application/rectangular-list-card.vue'
</script>

<style lang="scss" scoped>
.track-application {
  padding-top: 40px;
}
.breadcrumb {
  a,
  .active {
    text-decoration: none;
    color: #2c3e50;
    font-weight: 700;
  }
}
</style>
