<template>
  <div>
    <NavComponentVue />
    <router-view />
    <foot></foot>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>

<script setup>
import foot from '@/components/footer.vue'
import NavComponentVue from './components/NavComponent.vue'
</script>
