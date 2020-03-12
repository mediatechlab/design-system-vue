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
  background: #6524FB 0% 0% no-repeat padding-box;
  width: 98px;
  height: 42px;
  color: #fff;
  font-size: 14px;
  letter-spacing: 0;
  border: 0;
  border-radius: 100px;
  outline: 0;
}

.m_btn:hover {
  background: #B278F8 0% 0% no-repeat padding-box;
}

.m_btn:active {
  background: #A255FC 0% 0% no-repeat padding-box;
}

.m_btn:disabled {
  background: #F1EAFF 0% 0% no-repeat padding-box;
  color: #C4B9DB;
}

.m_btn::-moz-focus-inner {
  border: 0;
}
</style>
