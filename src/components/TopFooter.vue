<template>
  <div class="top-footer">
    <div class="left">
      <div class="top-footer__col">
        <h3>DC Comics</h3>
        <ul class="top-footer__col__menu">
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer linkddddddddddd</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
        </ul>
        <h3>Shop</h3>
        <ul class="top-footer__col__menu">
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer linkfffffff</a>
          </li>
        </ul>
      </div>
      <div class="top-footer__col">
        <h3>DC</h3>
        <ul class="top-footer__col__menu">
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer linkaaaaaaaaaaaaa</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
        </ul>
      </div>
      <div class="top-footer__col">
        <h3>Sites</h3>
        <ul class="top-footer__col__menu">
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
          <li>
            <a href="#">Footer link</a>
          </li>
        </ul>
      </div>
    </div>
    <div class="right"></div>
  </div>
</template>

<script>
export default {
  name: "TopFooter",
};
</script>
<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";
.top-footer {
  background-image: url("../assets/img/footer-bg.jpg");
  color: white;
  display: flex;
  &__col {
    margin-right: 2.4rem;
    a {
      color: lightgray;
    }
    a:hover {
      text-decoration: underline;
    }
  }
  .left {
    display: flex;
    justify-content: center;
    width: 40%;
    padding-bottom: 2rem;
    h3 {
      text-transform: uppercase;
      font-size: 1.8rem;
      padding: 2rem 0;
    }
    li {
      font-size: 0.8rem;
      padding: 0.3rem;
    }
  }
  .right {
    display: flex;
    justify-content: center;
    width: 60%;
    background-image: url("../assets/img/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-attachment: center;
    background-position: center;
    background-size: cover;
  }
}
</style>
