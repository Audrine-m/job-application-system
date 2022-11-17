<template>
  <div class="row">
    <div class="col-4">
      <img
        src="https://imgs.search.brave.com/TLwZghF8VFmxLjMzYA8SxE9it1NAPMBT6bR99T5WRow/rs:fit:711:225:1/g:ce/aHR0cHM6Ly90c2Ux/Lm1tLmJpbmcubmV0/L3RoP2lkPU9JUC5C/cllaRko5M3lGY0xX/Z1pNWTJTN3ZnSGFF/OCZwaWQ9QXBp"
        alt=""
      />
    </div>
    <div class="col-3">
      <div class="neffex">
        <span id="title"><slot name="job-title">python Developer</slot></span>
        <span class="children"
          ><i class="fa fa-building" aria-hidden="true" style="margin-right: 5px"></i
          ><slot name="company">safaricom</slot></span
        >
        <span class="children"
          ><i class="fa fa-map-marker" aria-hidden="true" style="margin-right: 5px"></i
          ><slot name="location">Nairobi</slot></span
        >
      </div>
    </div>
    <div class="col-5">
      <progressVue></progressVue>
    </div>
  </div>
</template>

<script setup>
import progressVue from './progress.vue'
</script>

<style lang="scss" scoped>
.row {
  box-shadow: rgba(0, 0, 0, 0.1) 0px 10px 50px;
  height: 200px;
  margin: 20px;
}
img {
  max-height: 200px;
  max-width: 100%;
  object-fit: cover;
}
.neffex {
  display: flex;
  flex-direction: column;
  text-align: left;
  justify-content: space-between;
  #title {
    font-size: 24px;
    font-weight: 800;
    margin-bottom: 10px;
    margin-top: 10px;
  }
  .children {
    color: orange;
    padding-top: 8px;
  }
}
</style>
