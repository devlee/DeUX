<template>
  <div class="home-index">
    <div class="h">
      <div class="n"></div>
      <div class="b"></div>
    </div>
    <div class="s">
      <div class="pws">
        <panel
          class="p"
          v-for="(item, idx) in Array.from({ length: 3 })"
          :key="item + idx"
        >
          <div class="pi">p1</div>
        </panel>
      </div>
    </div>
    <div class="c">
      <div class="pwc">
        <panel
          class="p"
          v-for="(item, idx) in Array.from({ length: 20 })"
          :key="item + idx"
        >
          <div class="pi">p1</div>
        </panel>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Panel from "../../layout/panel.vue";
export default defineComponent({
  name: "home-index",
  components: {
    Panel,
  },
  steup(props, context) {},
});
</script>
<style lang="less" scoped>
.home-index {
  height: 100%;
  width: 100%;
  color: red;
  display: grid;
  grid-template-columns: 25% auto;
  grid-template-rows: 320px auto;
  .h {
    grid-column-start: 1;
    grid-column-end: 3;
    // box-shadow: 0 0px 1px #e0e0e0;
  }
  .s {
    // box-shadow: 0 1px 1px #e0e0e0;
  }
  .s,
  .c {
    padding: 24px;
    // height: 100%;
    // overflow-y: auto;
  }
  .pws,
  .pwc {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-column-gap: 24px;
    grid-row-gap: 48px;
  }
  .pws {
    grid-template-columns: 1fr;
    grid-row-gap: 24px;
  }
  .p {
    flex: 1;
  }
  .pi {
    min-height: 300px;
  }
}
</style>
