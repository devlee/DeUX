<template>
  <div class="panel layout-el">
    <slot></slot>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  name: "panel",
  steup(props, context) {},
});
</script>
<style lang="less" scoped>
.panel {
  display: inline-block;
  overflow: hidden;
  border-radius: 12px;
  box-shadow: 2px 3px 8px #e0e0e0;
  background-color: #fff;
}
</style>
