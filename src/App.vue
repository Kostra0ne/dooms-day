<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">

* {
  box-sizing: border-box;
};

body {
  margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: whitesmoke;
  display: flex;
  align-items: flex-start;
  padding-top: 23vh;
  justify-content: center;
  height: 100vh;
  margin: 0;
  background: #4cc355;
  // background: linear-gradient(
  //   to bottom,
  //   #4cc355 0%,
  //   #fa6607 50%,
  //   #e2071c 100%
  // );
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#4cc355', endColorstr='#e2071c',GradientType=0 ); /* IE6-9 */
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
