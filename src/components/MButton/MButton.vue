<template>
  <button class="m_btn" :class="{ m_btn_shadow: shadow, m_btn_outline: outline, m_btn_none: none }" :disabled="disabled">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "m-button",
  props: {
    shadow: Boolean,
    outline: Boolean,
    disabled: Boolean,
    none: Boolean
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.m_btn {
  background: #6524fb 0% 0% no-repeat padding-box;
  height: 42px;
  color: #ffffff;
  font-size: 14px;
  letter-spacing: 0;
  border: 0;
  border-radius: 100px;
  outline: 0;
  vertical-align: middle;
  padding: 11px 26px;
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

.m_btn_shadow {
  box-shadow: 0px 3px 9px #00000014;
}

.m_btn_outline {
  border: 1px solid #651fff;
  background: none;
  color: #651fff;
}

.m_btn_outline:hover {
  background: #bb9bff59 0% 0% no-repeat padding-box;
}

.m_btn_outline:active {
  background: #a255fc8c 0% 0% no-repeat padding-box;
}

.m_btn_outline:disabled {
  background: #f1eaff 0% 0% no-repeat padding-box;
  border: 0;
}

.m_btn_none {
  border: none;
  background: none;
  color: #651fff;
}

.m_btn_none:hover {
  background: #bb9bff59 0% 0% no-repeat padding-box;
}

.m_btn_none:active {
  background: #a255fc8c 0% 0% no-repeat padding-box;
}

.m_btn_none:disabled {
  background: none;
  color: #c4b9db;
  border: 0;
}
</style>
