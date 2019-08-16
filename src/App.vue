<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>|
      <router-link to="/about">About</router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
@font-face {
  font-family: "Inconsolata";
  src: url("assets/Inconsolata-Regular.ttf") format("truetype");
}

@import "assets/color-scheme.scss";

body {
  background-color: $cs-main-dark;
  color: $cs-main-light;
}

#app {
  font-family: "Inconsolata", monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: $cs-main-light;
    &.router-link-exact-active {
      color: $cs-danger;
    }
  }
}
</style>
