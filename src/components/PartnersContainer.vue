<template>
  <section class="pt-5">
    <div class="container">
      <h1 class="text-center pb-4">Partners</h1>
      <p class="text-center">
        Leverage agile frameworks to provide a robust synopsis for high level
      </p>
      <p class="text-center">
        overviews. Iterative approaches to corporate stratergy.
      </p>
      <div class="box-img d-flex justify-content-center">
        <img
          v-for="(partner, i) in partners"
          :key="i"
          :src="`img/${partner}.png`"
          alt=""
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      partners: [
          'partner-2',
          'partner-3',
          'partner-4',
          'partner-5',
          'partner-6',
          'partner-8',
          'partner-1',
          'partner-7',
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/partnersContainer.scss";
</style>