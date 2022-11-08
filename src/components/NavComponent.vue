<template>
  <div class="container-fluid">
    <div id="nav">
      <nav class="d-flex justify-content-evenly">
        <div class="logo">
          <img src="../assets/jobs-remove.png" alt="logo" />
        </div>
        <div class="links">
          <router-link to="/">Home</router-link>
          <router-link to="/about">Find Jobs</router-link>
          <router-link to="/track-application">Track Application</router-link>
          <div class="auth">
            <router-link to="/sign-in">sign-in</router-link>
            <router-link to="/create-account"
              ><button class="c-account-btn">create-acoount</button></router-link
            >
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import '../styling/colors.scss';

nav {
  padding: 20px;
  background-color: $primary_color;
  // top: 0;
  margin: 0;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;

  .links {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    vertical-align: middle;
    margin-top: 10px;
  }
  .auth {
    margin-top: -2px;
    float: right;
    a {
      .c-account-btn {
        border: none;

        padding: 10px 40px;
        // top: -20px;
        vertical-align: middle;
        background: #08558f;
        border-radius: 8px;
        color: $tertiary_color;
        font-weight: bold;
        font-family: 'K2D';
        font-style: normal;
      }
      font-weight: bold;
      color: #2c3e50;
      padding-right: 40px;

      &.router-link-exact-active {
        color: $tertiary_color;
      }
    }
  }
  .logo {
    // width: 30%;
    img {
      position: absolute;
      width: 137px;
      height: 76px;
      top: -3px;
    }
  }

  a {
    font-weight: bold;
    color: #2c3e50;
    padding-right: 40px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande',
      'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 32px;
    text-decoration: none;
    &.router-link-exact-active {
      color: $tertiary_color;
      // text-decoration: underline;
    }
  }
}
</style>
