<template>
  <div class="about">
    <div class="sidebar">
      <h1>this is our sidebar</h1>

      <HelloWorld></HelloWorld>
    </div>
  </div>
</template>

<script setup>
import HelloWorld from '@/components/HelloWorld.vue'
</script>

<style lang="scss" scoped>
.center {
  display: flex;
  align-content: center;
  margin-left: 40%;
  margin-right: 30%;
}
</style>
