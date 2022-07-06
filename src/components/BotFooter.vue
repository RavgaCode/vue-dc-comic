<template>
  <section>
    <div class="container">
      <div class="footer-columns">
        <!-- BTN COL -->
        <div class="left-col">
          <div>
            <a href="#" class="footer-btn">SIGN-UP NOW!</a>
          </div>
        </div>
        <!-- SOCIALS COL -->
        <div class="right-col">
          <ul>
            <li><a href="#" class="follow-link">FOLLOW US</a></li>
            <li v-for="(social, index) in socials" :key="index">
              <a href="#"><img :src="social.img" :alt="social.alt" /></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BotFooter",
  data() {
    return {
      socials: [
        {
          img: require("../assets/img/footer-facebook.png"),
          alt: "Logo Facebook",
        },

        {
          img: require("../assets/img/footer-twitter.png"),
          alt: "Logo Twitter",
        },

        {
          img: require("../assets/img/footer-youtube.png"),
          alt: "Logo Youtube",
        },
        {
          img: require("../assets/img/footer-pinterest.png"),
          alt: "Logo Pinterest",
        },
        {
          img: require("../assets/img/footer-periscope.png"),
          alt: "Logo Periscope",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
section {
  background-color: #303030;
  height: 150px;
}
.footer-columns {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;
}
.footer-btn {
  color: white;
  font-weight: 800;
  padding: 1rem;
  border: 2px solid $brand-color;
}
.right-col ul {
  display: flex;
  align-items: center;

  li {
    padding-left: 0.5rem;
  }
}
.follow-link {
  color: $brand-color;
  font-weight: 800;
  font-size: 1.5rem;
}
</style>
