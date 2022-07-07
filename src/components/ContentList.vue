<template>
  <section>
    <div class="container">
      <div class="product-wrapper">
        <div class="card" v-for="(comic, index) in products" :key="index">
          <img :src="comic.thumb" :alt="comic.series" />
          <h4>{{ comic.series }}</h4>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import comics from "../assets/dc-comics.json";
export default {
  name: "ContentList",
  data() {
    return {
      products: comics,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

section {
  background-color: black;
  color: white;
}
.product-wrapper {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 2rem;
}
.card {
  width: calc(100% / 6 - 1rem);
  padding-bottom: 1.5rem;

  img {
    max-width: 100%;
  }
}
</style>
