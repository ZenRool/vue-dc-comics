<template>
  <li class="comic-card">
    <div class="comic-card__container">
      <img :src="cardObj.thumb" :alt="cardObj.series" />
    </div>
    <p>
      {{ cardObj.series }}
    </p>
  </li>
</template>
<script>
export default {
  name: "ComicCard",
  props: {
    cardObj: Object,
  },
};
</script>
<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";
@import "../style/button.scss";
.comic-card {
  color: white;
  width: 192px;
  margin: 1rem auto;
  display: flex;
  flex-direction: column;
  &__container {
    width: 192px;
    img {
      width: 192px;
      height: 200px;
      object-fit: cover;
      object-position: top;
    }
  }
  p {
    margin-top: 1rem;
    height: 3rem;
  }
}
</style>
