<template>
  <div class="prog">
    <div class="container">
      <span class="status">applied</span>
      <div class="spacebox"></div>
      <span class="status">received</span>
      <div class="spacebox"></div>
      <span class="status" v-if="accepted">accepted</span>
      <span class="status" v-else-if="accepted == false">rejected</span>
      <span class="status" v-else>waiting ..</span>
    </div>
    <div class="container margin-t">
      <div class="applied">
        <i class="fa fa-check" aria-hidden="true" style="color: white"></i>
      </div>

      <div class="lines"></div>
      <div class="received">
        <i class="fa fa-check" aria-hidden="true" style="color: white"></i>
      </div>
      <div class="lines"></div>
      <div v-if="accepted" :class="accepted ? 'accepted' : ''">
        <i class="fa fa-check" aria-hidden="true" style="color: white"></i>
      </div>
      <div></div>
      <div v-if="accepted == false" :class="accepted == false ? 'rejected' : ''">
        <i
          class="fa fa-exclamation-triangle"
          aria-hidden="true"
          style="color: white; font-size: 14px"
        ></i>
      </div>

      <div v-if="accepted == null" :class="accepted == null ? 'notyet' : ''">
        <div class="cover"></div>
      </div>
    </div>
  </div>
</template>

<script setup>
var accepted = true
var received = false
</script>

<style lang="scss" scoped>
@import '@/styling/colors.scss';
.margin-t {
  padding-left: 40px;
}
.container {
  margin-top: 30px;
  display: flex;
  flex-direction: row;
  .base {
    width: 20px;
    height: 20px;
    border-radius: 50%;
  }
  .applied {
    @extend .base;
    background-color: $applied_color;
  }
  .spacebox {
    width: 95px;
    height: 2px;
  }
  .lines {
    width: 130px;
    height: 1px;
    background-color: black;
    vertical-align: middle;
    margin-top: 10px;
  }
  .received {
    @extend .base;
    background-color: $received_color;
  }
  .accepted {
    @extend .base;
    background-color: green;
  }
  .rejected {
    @extend .base;
    background-color: red;
  }
  .notyet {
    @extend .base;
    background-color: black;
  }
  .cover {
    width: 16px;
    height: 16px;
    border-radius: 50%;
    background-color: white;

    margin-left: 2px;
    margin-top: 2px;
  }
  .status {
    font-weight: 600;
    font-size: 16px;
  }
}
</style>
