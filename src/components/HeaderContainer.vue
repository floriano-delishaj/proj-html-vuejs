<template>
  <header>
    <div class="filter">
      <nav-bar />
      <div class="container content-header text-center">
        <h1>Key to your success</h1>
        <p class="pt-4">
          EduPrime is the most versatible WordPress theme for educational
          pruposes, showcasing universities, courses, secondary schools etc.
        </p>
        <div class="buttons-header pt-3">
          <div class="btn">
            <i class="fas fa-search"></i>
            Search courses
          </div>
          <div class="btn">
            <i class="fas fa-user-plus"></i>
            Apply for university
          </div>
        </div>
      </div>

      <div class="wave">
        <img src="../../public/img/Wave-1.png" alt="" />
      </div>
    </div>
  </header>
</template>

<script>
import NavBar from "./NavBar.vue";
export default {
  components: {
    NavBar,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/headerContainer.scss";
</style>