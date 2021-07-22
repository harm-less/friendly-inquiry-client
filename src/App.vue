<template>
  <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
  <router-view />
</template>

<style lang="scss">
@import "scss-reset/_reset.scss";
@import url(https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;700&display=swap);

$media-desktop: "only screen and (max-width : 1024px)";
$media-tablet: "only screen and (max-width : 768px)";
$media-mobile: "only screen and (max-width : 600px)";
$media-mobile-sm: "only screen and (max-width : 480px)";

html,
body {
  background-color: #253b49;
  height: 100%;

  background-image: url(./assets/background.webp);
  background-size: 700px;
  background-position: center bottom;
  background-repeat: no-repeat;
  background-attachment: fixed;

  @media #{$media-mobile} {
    background-size: contain;
  }
}

#app {
  font-family: Open Sans, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
