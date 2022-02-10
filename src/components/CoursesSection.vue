<template>
  <section class="courses">
    <img class="w-100" src="../../public/svg/svg-1.svg" alt="" />
    <div class="container">
      <h1>Latest Courses</h1>
      <div class="row py-5">
        <div v-for="(item, i) in coursesInfo" :key="i" class="col-12 col-lg-3">
          <div class="card-box text-center">
            <img :src="`/img/${item.img}`" alt="" />
            <h5>{{ item.name }}</h5>
            <p>
              <span><i class="far fa-user"></i> Teacher: </span>
              <span>{{ item.teacher }}</span>
            </p>
            <p>
              <span><i class="far fa-money-bill-alt"></i> Price: </span>
              <span>{{ item.price }}</span>
            </p>
            <div class="btn red">
              <i class="far fa-eye"></i>
              View Course
            </div>
          </div>
        </div>
      </div>
      <img class="img pt-5 pb-2" src="/img/Exam-icon.png" alt="" />
      <div class="row">
        <div class="col-12 col-lg-6">
          <div class="box">
            <h1>The most efficient examination method</h1>
            <p class="py-4">
              EduPrime has gathered teachers from around the globe to brainstorm
              in oder to facilitate the evaluation of our students. Every
              teacher from our university has an influence on how students are
              evaluated at his/her subject.
            </p>
            <div class="btn red">Discover the Method</div>
          </div>
        </div>

        <div class="col-12 col-lg-6">
          <div class="box">
            <img
              class="img-fluid"
              src="../../public/img/Exam-Illustration.png"
              alt=""
            />
          </div>
        </div>
      </div>
      <div class="row pt-5">
        <div class="col-12 col-lg-6">
          <div class="box">
            <img
              class="img-fluid"
              src="../../public/img/Girl-Illustration.png"
              alt=""
            />
          </div>
        </div>
        <div class="col-12 col-lg-6">
          <div class="box">
              <img class="img pb-4" src="../../public/img/Exam-icon-1.png" alt="" />
            <h1>Variable fees for international students</h1>
            <p class="py-4">
              EduPrime has gathered teachers from around the globe to brainstorm
              in oder to facilitate the evaluation of our students. Every
              teacher from our university has an influence on how students are
              evaluated at his/her subject.
            </p>
            <div class="btn red">List of fees</div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      coursesInfo: [
        {
          img: "Decisions-icon.png",
          name: "Make Better Decision",
          teacher: "James Collins",
          price: "$21.00",
        },
        {
          img: "Speaker-icon.png",
          name: "How to be a speaker",
          teacher: "James Collins",
          price: "Free",
        },
        {
          img: "Network-icon.png",
          name: "Network Introductions",
          teacher: "James Collins",
          price: "Free",
        },
        {
          img: "Brand-icon.png",
          name: "Brand Management",
          teacher: "James Collins",
          price: "Free",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/coursesSection.scss";
</style>