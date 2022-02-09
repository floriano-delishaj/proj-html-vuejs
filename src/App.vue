<template>
  <div id="app">
    <header-container />
    <main-container />
  </div>
</template>

<script>

import HeaderContainer from "./components/HeaderContainer.vue";
import MainContainer from './components/MainContainer.vue';

export default {
  name: "App",
  components: {
    HeaderContainer,
    MainContainer,
  },
};
</script>

<style lang="scss">
@import "@/style/main.scss";
</style>
