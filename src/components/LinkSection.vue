<template>
  <section>
    <div class="container">
      <div class="link-columns">
        <div class="link-col">
          <!-- LINK COLS -->
          <div class="first-col">
            <h2>DC COMICS</h2>
            <ul>
              <li v-for="(link, index) in comics" :key="index">
                <a href="link.link">{{ link.text }}</a>
              </li>
            </ul>
            <h2>SHOP</h2>
            <ul v-for="(link, index) in shop" :key="index">
              <li>
                <a href="link.link">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="second-col">
            <h2>DC</h2>
            <ul>
              <li v-for="(link, index) in dc" :key="index">
                <a href="link.link">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="third-col">
            <h2>SITES</h2>
            <ul>
              <li v-for="(link, index) in sites" :key="index">
                <a href="link.link">{{ link.text }}</a>
              </li>
            </ul>
          </div>
        </div>
        <!-- IMG COL -->
        <div class="img-col">
          <img src="../assets/img/dc-logo-bg.png" alt="DC Logo" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "LinkSection",
  data() {
    return {
      comics: [
        {
          text: "Characters",
          link: "#",
        },
        {
          text: "Comics",
          link: "#",
        },
        {
          text: "Movies",
          link: "#",
        },
        {
          text: "TV",
          link: "#",
        },
        {
          text: "Games",
          link: "#",
        },
        {
          text: "Videos",
          link: "#",
        },
        {
          text: "News",
          link: "#",
        },
      ],
      shop: [
        {
          text: "Shop DC",
          link: "#",
        },
        {
          text: "Shop DC Collectibles",
          link: "#",
        },
      ],
      dc: [
        {
          text: "Term Of Use",
          link: "#",
        },
        {
          text: "Privacy policy (New)",
          link: "#",
        },
        {
          text: "Ad Choices",
          link: "#",
        },
        {
          text: "Advertising",
          link: "#",
        },
        {
          text: "Jobs",
          link: "#",
        },
        {
          text: "Subscriptions",
          link: "#",
        },
        {
          text: "Talent Workshops",
          link: "#",
        },
        {
          text: "CPSC Certificates",
          link: "#",
        },
        {
          text: "Ratings",
          link: "#",
        },
        {
          text: "Shop Help",
          link: "#",
        },
        {
          text: "Contact Us",
          link: "#",
        },
      ],
      sites: [
        {
          text: "DC",
          link: "#",
        },
        {
          text: "MAD Magazine",
          link: "#",
        },
        {
          text: "DC Kids",
          link: "#",
        },
        {
          text: "DC Universe",
          link: "#",
        },
        {
          text: "DC Power Visa",
          link: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

section {
  background-image: url(../assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 400px;
}
.link-columns {
  display: flex;
  justify-content: space-between;

  h2 {
    color: white;
    padding: 1.5rem 0;
  }
  a {
    color: $main-text-color;
  }
}
.link-col {
  display: flex;
  padding: 1rem 0;

  div {
    padding-right: 3rem;
  }
}
.img-col {
  position: relative;
  height: 400px;
  img {
    display: block;
    height: 100%;
    width: 600px;
    overflow: hidden;
    object-fit: none;
  }
}
</style>
