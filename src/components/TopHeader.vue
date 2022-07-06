<template>
  <section>
    <div class="container">
      <div class="header-columns">
        <div class="left-col">
          <img src="../assets/img/dc-logo.png" alt="Logo DC" />
        </div>
        <div class="right-col">
          <ul>
            <li
              v-for="(link, index) in nav"
              :key="index"
              :class="{ active: link.active }"
            >
              <a :href="link.link">{{ link.text }}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "TopHeader",
  data() {
    return {
      nav: [
        {
          text: "CHARACTERS",
          link: "#",
          active: false,
        },
        {
          text: "COMICS",
          link: "#",
          active: true,
        },
        {
          text: "MOVIES",
          link: "#",
          active: false,
        },
        {
          text: "TV",
          link: "#",
          active: false,
        },
        {
          text: "GAMES",
          link: "#",
          active: false,
        },
        {
          text: "COLLECTIBLES",
          link: "#",
          active: false,
        },
        {
          text: "VIDEOS",
          link: "#",
          active: false,
        },
        {
          text: "FANS",
          link: "#",
          active: false,
        },
        {
          text: "NEWS",
          link: "#",
          active: false,
        },
        {
          text: "SHOP",
          link: "#",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
section {
  height: 150px;
  margin-bottom: 5px;
}
.header-columns {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
ul {
  display: flex;
}
li {
  padding: 0 0.8rem;
  line-height: 150px;
  display: block;

  a {
    color: $main-text-color;
    font-weight: 800;
  }
}
.active {
  border-bottom: 5px solid $brand-color;
}
</style>
