<template>
  <div class="container-fluid">
    <div class="cat">
      <h3 id="header">Browse By Job <span id="category">Categories</span></h3>
      <p class="container">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut et massa mi. Aliquam
        in hendrerit urna. Pellentesque sit amet sapien fringilla, mattis li. Lorem ipsum
        dolor sit amet consectetur adipisicing elit. Harum labore architecto sint eius et
        at sapiente deserunt repellat voluptatum sunt, laudantium neque facere modi
        ratione assumenda. Numquam distinctio reiciendis id.
      </p>
      <div class="container box">
        <div class="row">
          <card>
            <template v-slot:title> Design & Development </template>
          </card>
          <card>
            <template v-slot:title> Design & Development </template>
          </card>

          <card>
            <template v-slot:icon>
              <i
                class="fa fa-envelope-open"
                aria-hidden="true"
                style="font-size: 41px"
              ></i>
            </template>
            <template v-slot:title> Fashion & Design </template>
          </card>
          <card>
            <template v-slot:icon>
              <i
                class="fa fa-envelope-open"
                aria-hidden="true"
                style="font-size: 41px"
              ></i>
            </template>
            <template v-slot:title> Fashion & Design </template>
          </card>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import card from './widgets/cards.vue'
</script>

<style lang="scss" scoped>
@import url(../../styling/colors.scss);

.row {
  display: Flex;
  justify-content: space-between;
}

#category {
  color: #0a9fe8;
}
#header {
  font-weight: 600;
}

.box {
  padding: 25px;
}
.cat {
  background-color: aliceblue;
  padding: 40px;
  margin-top: 70px;
}
</style>
