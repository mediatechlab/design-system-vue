<template>
  <div id="app">
    <div id="buttons">
      <h1>Buttons</h1>

      <div id="buttons__container">
        <div class="container__top">
          <m-button>Primary - No Shadow</m-button>
          <m-button shadow>Primary - With Shadow</m-button>
          <m-button outline>Primary - With Outline</m-button>
          <m-button none>Primary - None</m-button>
        </div>

        <div class="container__bottom">
          <m-button disabled>Primary - No Shadow - Disabled</m-button>
          <m-button disabled shadow>Primary - With Shadow - Disabled</m-button>
          <m-button disabled outline>Primary - With Outline - Disabled</m-button>
          <m-button disabled none>Primary - None - Disabled</m-button>
        </div>
      </div>
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

#buttons {
  display: flex;
  flex-direction: column;
  flex: 1;
}

#buttons h1 {
  font-size: 60px;
  color: #443665;
  border-bottom: 1px;
  border-bottom-color: #707070;
  border-bottom-style: dashed;
  padding-bottom: 30px;
}

#buttons__container {
  display: flex;
  flex-direction: column;
}

#buttons__container button {
  margin: 5px;
}
</style>
