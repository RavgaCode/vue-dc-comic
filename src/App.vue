<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <!-- HEADER -->
    <TopHeader />
    <main>
      <ContentList />
    </main>
    <!-- FOOTER -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import TopHeader from "./components/TopHeader.vue";
import ContentList from "./components/ContentList.vue";
export default {
  name: "App",
  components: {
    TopHeader,
    ContentList,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
#app {
}
</style>
