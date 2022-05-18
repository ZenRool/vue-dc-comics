<template>
  <div class="jumbo"></div>
</template>
<script>
export default {
  name: "MyJumbo",
};
</script>
<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";
.jumbo {
  background-image: url("../assets/img/jumbotron.jpg");
  background-repeat: no-repeat;
  background-position: top;
  background-size: cover;
  height: 400px;
}
</style>
