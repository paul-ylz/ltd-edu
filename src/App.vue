<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "app",
  components: {
    HelloWorld
  },
  metaInfo: {
    title: "foo bar",
    titleTemplate: "%s - Yay!",
    meta: [
      {
        vmid: "og:title",
        property: "og:title",
        content: "Test title",
        template: chunk => `${chunk} - My page` // or as string template: '%s - My page'
      }
    ]
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
