<template>
  <header class="header">
    <div class="header__logo">
      <img src="../assets/img/dc-logo.png" alt="logo dc comics" />
    </div>
    <nav>
      <ul class="header__menu">
        <li
          v-for="(item, index) in links"
          :key="index"
          :class="{ active: item.active }"
          @click="activeIndex(index)"
        >
          <a href="javascript: void(0)">{{ item.text }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "MyHeader",
  data: function () {
    return {
      links: [
        {
          url: "#",
          text: "Character",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: true,
        },
        {
          url: "#",
          text: "Movies",
          active: false,
        },
        {
          url: "#",
          text: "Tv",
          active: false,
        },
        {
          url: "#",
          text: "Games",
          active: false,
        },
        {
          url: "#",
          text: "Collectibles",
          active: false,
        },
        {
          url: "#",
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "Fans",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
        {
          url: "#",
          text: "Shop",
          active: false,
        },
      ],
    };
  },
  methods: {
    activeIndex: function (index) {
      for (let i = 0; i < this.links.length; i++) {
        this.links[i].active = false;
      }
      this.links[index].active = true;
    },
  },
};
</script>
<style lang="scss">
@import "../style/common.scss";
@import "../style/variables.scss";
.header {
  display: flex;
  height: 100px;
  &__logo {
    width: 45%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    img {
      height: 60%;
    }
  }
  &__menu {
    width: 55%;
    display: flex;
    justify-content: flex-start;
    align-items: stretch;
    height: 100%;
    li {
      position: relative;
      display: flex;
      align-items: center;
      margin: 0 0.5rem;
      &.active::after {
        content: "";
        height: 100%;
        width: calc(100% - 10px);
        position: absolute;
        right: 5px;
        border-bottom: 5px solid $brand-primary-color;
      }
      a {
        color: $text-color;
      }
    }
  }
}
</style>
