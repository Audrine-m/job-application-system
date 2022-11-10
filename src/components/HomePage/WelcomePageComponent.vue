<script setup>
import searchComponent from '@/components/searchbarComponent.vue'
</script>

<style lang="scss" scoped>
@import url(../../styling/colors.scss);
</style>

<style lang="scss" scoped>
.container {
  padding-top: 50px;
}

.welcome {
  // width: 60%;
  padding: 30px;
  small {
    float: left;
    padding-left: 2px;
  }
  .welcome-text {
    font-weight: 700;
    font-size: 56px;
    text-align: start;
    word-spacing: 6px;
  }
}
</style>

<template>
  <div class="container">
    <div class="row">
      <div class="col-lg-6">
        <div class="welcome">
          <h1 class="welcome-text">We Help You Find Your Dream Job</h1>
          <small>Our Wolrd class services will help you land your dream job</small>
        </div>
        <searchComponent />
      </div>
      <div class="col-lg-6">
        <img src="@/assets/welcome.svg" alt="welcome-image" />
      </div>
    </div>
  </div>
</template>
