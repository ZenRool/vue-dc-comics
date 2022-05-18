<template>
  <div class="panel">
    <ul class="panel__menu">
      <li v-for="(item, index) in buys" :key="index">
        <div class="img-container">
          <img
            :src="require(`../assets/img/buy-${item.src}`)"
            alt="item.text"
          />
        </div>
        <p>
          {{ item.text }}
        </p>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "MenuPanel",
  data: function () {
    return {
      buys: [
        {
          url: "#",
          text: "Visa",
          src: "dc-power-visa.svg",
        },
        {
          url: "#",
          text: "Subsriptoins",
          src: "comics-subscriptions.png",
        },
        {
          url: "#",
          text: "locator",
          src: "comics-shop-locator.png",
        },
        {
          url: "#",
          text: "mershandise",
          src: "comics-merchandise.png",
        },
        {
          url: "#",
          text: "comics",
          src: "comics-digital-comics.png",
        },
      ],
    };
  },
};
</script>
<style lang="scss">
@import "../style/common.scss";
@import "../style/variables.scss";
.panel {
  display: flex;
  height: 300px;
  background-color: $brand-primary-color;
  color: white;
  width: 100%;
  &__menu {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    li {
      .img-container {
        height: 200px;
        width: 100px;
        margin-right: 1rem;
        display: flex;
        align-items: center;
      }
      margin: 0 2rem;
      position: relative;
      display: flex;
      align-items: center;
    }
  }
}
</style>
