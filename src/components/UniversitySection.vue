<template>
  <section class="university">
    <div class="university-container container">
      <div class="d-flex flex-column align-items-center">
        <img class="img" src="/img/Clock-and-Bell.png" alt="" />
        <h1 class="title">University Year</h1>
        <div class="container-card d-flex w-75 pt-5 justify-content-end">
          <div class="text-card">
            <h5>Demo Classes</h5>
            <p>
              In the first week, students try to accommodate with the teaching
              style and choose their optional courses.
            </p>
          </div>
          <div class="text-card">
            <h5>Graduation Day</h5>
            <p>
              On the day of graduation, all students gather for the ceremony and
              then network and party among others.
            </p>
          </div>
        </div>
        <img src="/img/Timeline-Item.png" alt="" />
        <div class="container-card d-flex w-75">
          <div class="text-card">
            <h5>Demo Classes</h5>
            <p>
              In the first week, students try to accommodate with the teaching
              style and choose their optional courses.
            </p>
          </div>
          <div class="text-card">
            <h5>Graduation Day</h5>
            <p>
              On the day of graduation, all students gather for the ceremony and
              then network and party among others.
            </p>
          </div>
        </div>
        <img
          class="img pt-5"
          src="/img/upcoming-events-calendar-icon.png"
          alt=""
        />
        <h1>Upcoming Events</h1>
      </div>
      <div class="row pt-5">
        <div v-for="(item, i) in events" :key="i" class="col-12 col-lg-4">
          <div class="event-card text-center">
            <h3>{{ item.title }}</h3>
            <p class="py-1">
              <i class="far fa-calendar-alt"></i>
              {{ item.date }}
            </p>
            <p>
              {{ item.content }}
            </p>
            <div>
              <div class="btn red">
                <i class="fas fa-plus"></i>
                {{item.button}}
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="d-flex justify-content-center pt-5 mt-5">
        <div class="btn">View All Events</div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      events: [
        {
          title: "Coaching Sessions",
          date: "20 May 21:30 PM",
          content:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sit natus illum ex [...]",
          button: 'Find more'
        },
        {
          title: "Coaching Sessions",
          date: "20 May 21:30 PM",
          content:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sit natus illum ex [...]",
          button: 'Find more'
        },
        {
          title: "Coaching Sessions",
          date: "20 May 21:30 PM",
          content:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sit natus illum ex [...]",
          button: 'Find more'
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/universitySection.scss";
</style>