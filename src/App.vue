<template>
  <home />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Home from "./components/pages/home/home-index.vue";

export default defineComponent({
  name: "App",
  components: {
    Home,
  },
});
</script>

<style>
* {
  box-sizing: border-box;
}
html,
body {
  margin: 0;
  padding: 0;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #fefefe;
  height: 100%;
  width: 100%;
}
#app {
  height: 100%;
  width: 100%;
}
</style>
