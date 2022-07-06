<template>
  <section>
    <div class="container">
      <h2>---> Content goes here</h2>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContentList",
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

section {
  background-color: black;
  color: white;
  height: 80px;
}
h2 {
  line-height: 80px;
}
</style>
