<template>
  <div id="app">
    <div id="buttons">
      <h1>Buttons</h1>
      <m-button>Sign up</m-button>
    </div>
  </div>
</template>

<script>
import { MButton } from "./components";

export default {
  name: "App",
  components: {
    MButton
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 60px 60px 0 60px;
}

#buttons h1 {
  font-size: 60px;
  color: #443665;
  border-bottom: 1px;
  border-bottom-color: #707070;
  border-bottom-style: dashed;
  padding-bottom: 30px;
}
</style>
