<template>
  <section class="faculties">
    <h1 class="text-center">Faculties available at EduPrime</h1>
    <p class="text-center pt-4">
      A single university with a load of courses, tailored
    </p>
    <p class="text-center">to satisfy any student's needs.</p>

    <div class="menu mt-5">
      <div class="container d-flex">
        <div
          v-for="(card, i) in faculties"
          :key="i"
          class="
            card-box
            d-flex
            flex-column
            align-items-center
            justify-content-center
          "
        >
          <img :src="`/img/${card.img}`" alt="" />
          <p class="text-center">{{card.content}}</p>
        </div>
      </div>
    </div>

    <div class="container mt-5">
      <div class="row">
        <div class="col-12 col-lg-6">
          <img
            class="img-fluid"
            src="/img/Gavel-Illustration-e1556884768193.png"
            alt=""
          />
        </div>

        <div class="col-12 col-lg-6 d-flex flex-column justify-content-between">
          <h1>Law Faculty</h1>
          <p>
            Learning from world-leading academics and practioners, you'll not
            only receive an outstanding grounding in the theory of law, but you
            will be able to understand how those principles are applied in
            practice through a range of student-led activities and competitions.
          </p>
          <div>
            <div class="btn red">Read More</div>
          </div>
        </div>
      </div>
    </div>

    <img class="sticky-bottom w-100" src="/svg/svg-0.svg" alt="" />
  </section>
</template>

<script>
export default {
  data() {
    return {
      faculties: [
        {
          img: "Gavel-v2.png",
          content: "Law Faculty",
        },
        {
          img: "Coins-tabs-v2.png",
          content: "Economy",
        },
        {
          img: "Medicine-tabs-v2.png",
          content: "Medicine",
        },
        {
          img: "Computer-tabs-v2.png",
          content: "Computer Science",
        },
        {
          img: "Palette-tabs-v2.png",
          content: "Graphic Design",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/facultiesSection.scss";
</style>