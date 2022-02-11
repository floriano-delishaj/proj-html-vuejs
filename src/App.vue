<template>
  <div id="app">
    <header-container />
    <main-container />
    <footer-content />
  </div>
</template>

<script>
import "dayjs/locale/es";

import HeaderContainer from "./components/HeaderContainer.vue";
import MainContainer from "./components/MainContainer.vue";
import FooterContent from './components/footerContent.vue';

export default {
  name: "App",
  components: {
    HeaderContainer,
    MainContainer,
    FooterContent,
  },
};
</script>

<style lang="scss">
@import "@/style/main.scss";
</style>
