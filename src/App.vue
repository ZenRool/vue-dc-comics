<template>
  <div id="app">
    <!-- Header -->
    <MyHeader />
    <main>
      <MyJumbo />
      <MenuPanel />
    </main>
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyJumbo from "./components/MyJumbo.vue";
import MenuPanel from "./components/MenuPanel.vue";
export default {
  name: "App",
  components: {
    MyHeader,
    MenuPanel,
    MyJumbo,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
