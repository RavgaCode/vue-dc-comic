<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <!-- HEADER -->
    <TopHeader />
    <main>
      <ContentList />
      <BlueBand />
      <LinkSection />
    </main>
    <!-- FOOTER -->
    <BotFooter />
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import TopHeader from "./components/TopHeader.vue";
import ContentList from "./components/ContentList.vue";
import BlueBand from "./components/BlueBand.vue";
import LinkSection from "./components/LinkSection.vue";
import BotFooter from "./components/BotFooter.vue";
export default {
  name: "App",
  components: {
    TopHeader,
    ContentList,
    BlueBand,
    LinkSection,
    BotFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
#app {
}
</style>
