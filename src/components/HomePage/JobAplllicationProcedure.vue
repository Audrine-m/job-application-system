<template>
  <div class="container">
    <div class="intro-text">
      <h3 class="welcome-text">Find your Job In Three easy steps</h3>
      <small
        >Post a job to tell us about your project. We will quickly match you with the
        right freelancers </small
      ><br />

      <div class="row">
        <!-- <ol>
          <li></li>
          <li></li>
          <li></li>
        </ol> -->
        <div class="col-lg-6">
          <div class="row padding-top">
            <div class="col-12 float-left">
              <div class="title"><span class="number">1</span> Register an account</div>
              <small class="padding-left"
                >Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos et
                earum vitae quam iusto id ut eum, reiciendis aperiam aliquid cupiditate
                esse debitis illo unde animi velit minima? Possimus, maxime!</small
              >
            </div>

            <div class="col-12 float-left">
              <div class="title"><span class="number">2</span> Find your job</div>
              <small class="padding-left"
                >Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos et
                earum vitae quam iusto id ut eum, reiciendis aperiam aliquid cupiditate
                esse debitis illo unde animi velit minima? Possimus, maxime!</small
              >
            </div>

            <div class="col-12 float-left">
              <div class="title"><span class="number">3</span> Apply for job</div>
              <small class="padding-left"
                >Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos et
                earum vitae quam iusto id ut eum, reiciendis aperiam aliquid cupiditate
                esse debitis illo unde animi velit minima? Possimus, maxime!</small
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
@import '../../styling/colors.scss';

small {
  float: left;
  padding-left: 2px;
}
.welcome-text {
  font-weight: 700;
  font-size: 44px;
  text-align: start;
  word-spacing: 6px;
}
.intro-text {
  display: block;
}
.float-left {
  float: left;
  text-align: start;
}
.title {
  font-weight: 600;
  font-size: 16px;
}
.title:hover {
  color: $secondary_color;
  .number {
    border-radius: 50%;
    background-color: $secondary_color;
    color: white;
  }
}
.padding-left {
  padding-left: 40px;
  font-size: 13px;
}
.padding-top {
  padding-top: 40px;
}
</style>
