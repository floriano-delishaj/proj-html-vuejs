<template>
  <div>
    <info-courses />
    <faculties-section />
    <university-section />
    <courses-section />
    <news-letter />
    <partners-container />
  </div>
</template>

<script>
import CoursesSection from "./CoursesSection.vue";
import FacultiesSection from "./FacultiesSection.vue";
import InfoCourses from "./InfoCourses.vue";
import NewsLetter from './NewsLetter.vue';
import PartnersContainer from './PartnersContainer.vue';
import UniversitySection from "./UniversitySection.vue";

export default {
  components: {
    InfoCourses,
    FacultiesSection,
    UniversitySection,
    CoursesSection,
    NewsLetter,
    PartnersContainer,
  },
};
</script>

<style lang="scss">
body {
  background-color: #f7f8fa;
}

.img {
  width: 70px;
}
</style>