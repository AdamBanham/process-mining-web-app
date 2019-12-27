<template>
  <div id="app">
    <div id="nav">
      <router-link to="/welcome">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/">Login</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  color: snow;
  a {
    font-weight: bold;
    color: snow;

    &.router-link-exact-active {
      color: #526AC0;
    }
  }
}

html {
  background-color: #332E30 !important;
}
</style>
