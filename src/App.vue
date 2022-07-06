<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <!-- HEADER -->
    <TopHeader />
    <main>
      <ContentList />
      <BlueBand />
    </main>
    <!-- FOOTER -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import TopHeader from "./components/TopHeader.vue";
import ContentList from "./components/ContentList.vue";
import BlueBand from "./components/BlueBand.vue";
export default {
  name: "App",
  components: {
    TopHeader,
    ContentList,
    BlueBand,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
#app {
}
</style>
