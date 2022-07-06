<template>
  <section>
    <div class="container">
      <ul>
        <li v-for="(icon, index) in icons" :key="index">
          <img :src="icon.iconPath" :alt="icon.iconAlt" />
          <a :href="icon.link">{{ icon.text }}</a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "BlueBand",
  data() {
    return {
      icons: [
        {
          text: "DIGITAL COMICS",
          iconPath: require("../assets/img/buy-comics-digital-comics.png"),
          link: "#",
          iconAlt: "Buy Digital",
        },
        {
          text: "DC MERCHANDISE",
          iconPath: require("../assets/img/buy-comics-merchandise.png"),
          link: "#",
          iconAlt: "Buy Merchandise",
        },
        {
          text: "SUBSCRIPTION",
          iconPath: require("../assets/img/buy-comics-subscriptions.png"),
          link: "#",
          iconAlt: "Buy Subscription",
        },
        {
          text: "COMIC SHOP LOCATOR",
          iconPath: require("../assets/img/buy-comics-shop-locator.png"),
          link: "#",
          iconAlt: "Shop Locator",
        },
        {
          text: "DC POWER VISA",
          iconPath: require("../assets/img/buy-dc-power-visa.svg"),
          link: "#",
          iconAlt: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
section {
  background-color: $brand-color;
  height: 150px;
}
ul {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;

  img {
    height: 50px;
  }
  li {
    display: flex;
    align-items: center;
    padding: 0 1rem;
  }
  a {
    color: white;
    padding: 0 0.5rem;
  }
}
</style>
