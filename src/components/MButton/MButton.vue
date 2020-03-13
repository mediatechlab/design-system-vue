<template>
  <button class="m_btn">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "m-button",
  props: {
    small: Boolean
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.m_btn {
  background: #6524fb 0% 0% no-repeat padding-box;
  width: 98px;
  height: 42px;
  color: #ffffff;
  font-size: 14px;
  letter-spacing: 0;
  border: 0;
  border-radius: 100px;
  outline: 0;
  vertical-align: middle;
}

.m_btn:hover {
  background: #b278f8 0% 0% no-repeat padding-box;
}

.m_btn:active {
  background: #a255fc 0% 0% no-repeat padding-box;
}

.m_btn:disabled {
  background: #f1eaff 0% 0% no-repeat padding-box;
  color: #c4b9db;
}

.m_btn::-moz-focus-inner {
  border: 0;
}
</style>
