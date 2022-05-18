<template>
  <div id="app">
    <!-- Header -->
    <MyHeader />
    <main>
      <MyJumbo />
      <MenuPanel />
    </main>
    <footer><TopFooter /></footer>
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyJumbo from "./components/MyJumbo.vue";
import MenuPanel from "./components/MenuPanel.vue";
import TopFooter from "./components/TopFooter.vue";
export default {
  name: "App",
  components: {
    MyHeader,
    MenuPanel,
    MyJumbo,
    TopFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
