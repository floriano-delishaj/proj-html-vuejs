<template>
  <nav class="navbar navbar-expand-lg">
    <a class="navbar-brand" href="#">
      <img
        src="/img/theme_eduprime_logo.png"
        width="300"
        class="d-inline-block align-top"
        alt=""
      />
    </a>
    <button
      @click="openModal()"
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarNav"
      aria-controls="navbarNav"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <i class="fas fa-bars"></i>
    </button>
    <div
      :class="{ show: modal }"
      class="collapse navbar-collapse justify-content-end"
      id="navbarNav"
    >
      <ul class="navbar-nav">
        <li v-for="(item, i) in navList" :key="i" class="nav-item">
          <a class="nav-link" href="#">{{ item }}</a>
        </li>
      </ul>
      <div class="btn">VIEW COURSES</div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      modal: false,
      navList: [
        "Home",
        "Courses",
        "About Us",
        "News",
        "Pages",
        "Contact",
        "Purchase",
      ],
    };
  },
  methods: {
    openModal() {
      this.modal = !this.modal;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/navBar.scss";
</style>