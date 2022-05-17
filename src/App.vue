<template>
  <div id="app">
    <!-- Header -->
    <MyHeader />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";

export default {
  name: "App",
  components: {
    MyHeader,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
