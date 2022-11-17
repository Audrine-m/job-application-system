<template>
  <div class="card shadow">
    <div class="card-body">
      <div class="icon float-left">
        <slot name="icon"
          ><i class="fa fa-twitter" aria-hidden="true" style="font-size: 41px"></i
        ></slot>
      </div>
      <div class="titl float-left">
        <h5 class="card-title"><slot name="title">title</slot></h5>
      </div>
      <div class="sub float-left">
        <h6 class="card-subtitle mb-2 text-muted float-left">
          <slot name="posts">15k+ Job Posts</slot>
        </h6>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.shadow {
  border: none;
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  width: 240px;
  height: 200px;
  border-radius: 8px;
  margin: 20px;
}
.card-title {
  font-weight: 800;
  font-size: 24px;
}
.i {
  font-size: 41px;
  margin-bottom: 20px;
}
.float-left {
  float: left;
  text-align: left;
}
.icon {
  margin-bottom: 20px;
}
</style>
