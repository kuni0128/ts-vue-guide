<template>
  <div id="app">
    <span :title="message">
      Hover your mouse over me for a few seconds to see my dynamically bound
      title!
    </span>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
export default class App extends Vue {
  private message = "You loaded this page on " + new Date().toLocaleString();
}
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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
