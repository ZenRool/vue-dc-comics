<template>
  <div id="app">
    <!-- Header -->
    <MyHeader />
    <main>
      <MyJumbo />
      <ComicLine />
      <MenuPanel />
    </main>
    <footer>
      <TopFooter />
      <BottomFooter />
    </footer>
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyJumbo from "./components/MyJumbo.vue";
import MenuPanel from "./components/MenuPanel.vue";
import TopFooter from "./components/TopFooter.vue";
import BottomFooter from "./components/BottomFooter.vue";
import ComicLine from "./components/ComicLine.vue";
export default {
  name: "App",
  components: {
    MyHeader,
    MenuPanel,
    MyJumbo,
    TopFooter,
    BottomFooter,
    ComicLine,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
