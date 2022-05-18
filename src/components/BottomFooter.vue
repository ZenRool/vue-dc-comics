<template>
  <div class="bottom-footer">
    <div class="left">
      <button>Sing-up now!</button>
    </div>
    <div class="right">
      <h2>Follow us</h2>
      <div
        v-for="(social, index) in socials"
        class="img-container"
        :key="index"
      >
        <img
          :src="require(`../assets/img/footer-${social.src}.png`)"
          alt="item.text"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "BottomFooter",
  data: function () {
    return {
      socials: [
        {
          url: "#",
          text: "FacciaLibro",
          src: "facebook",
        },
        {
          url: "#",
          text: "Twitttt",
          src: "twitter",
        },
        {
          url: "#",
          text: "Il tubo",
          src: "youtube",
        },
        {
          url: "#",
          text: "le foto",
          src: "pinterest",
        },
        {
          url: "#",
          text: "Ciao",
          src: "periscope",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";
@import "../style/button.scss";
.bottom-footer {
  background-color: $brand-secondary-color;
  height: 80px;
  display: flex;
  align-items: center;
  .left {
    width: 40%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .right {
    h2 {
      color: $brand-primary-color;
    }
    width: 60%;
    display: flex;
    justify-content: center;
    align-items: center;
    .img-container {
      margin: 0 0.8rem;
    }
  }
}
</style>
