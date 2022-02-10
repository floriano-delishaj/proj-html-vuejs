<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col-12 col-lg-4">
          <div class="card-box d-flex flex-column justify-content-between">
            <img src="/img/theme_eduprime_logo.png" alt="" />
            <p>
              EduPrime is the most versatile WordPress theme for educational
              purposes, showcasing universities, courses, secondary schools etc.
            </p>
            <div class="socials">
              <a href="#">
                <i class="fab fa-facebook-f fa-fw"></i>
              </a>
              <a href="#">
                <i class="fab fa-twitter fa-fw"></i>
              </a>
              <a href="#">
                <i class="fab fa-instagram fa-fw"></i>
              </a>
            </div>
          </div>
        </div>

        <div class="col-12 col-lg-4">
          <div class="card-box d-flex">
            <ul v-for="(list, i) in listUl" :key="i">
              <li>
                <h5>{{ list.title }}</h5>
              </li>

              <li v-for="(argoments, i) in list.argoments" :key="i">
                {{ argoments }}
              </li>
            </ul>
          </div>
        </div>

        <div class="col-12 col-lg-4">
          <div class="card-box d-flex flex-column align-items-end justify-content-between">
            <div class="input-container">
              <input type="text" placeholder="Search..." />
              <div class="btn">
                <i class="fas fa-search fa-fw"></i>
              </div>
            </div>

            <h5>Seach categories</h5>

            <div class="categories d-flex flex-wrap justify-content-end">
                <div v-for="(category, i) in categories" :key="i">
                    {{category}}
                </div>
            </div>

            <p class="copyright">ModelTheme. All rights reserved.</p>
          </div>
        </div>
      </div>

      <div class="btn">
          <a href="#">
              <i class="fas fa-angle-up fa-fw"></i>
          </a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      listUl: [
        {
          title: "Get EduPrime",
          argoments: [
            "Request a website",
            "Browse Themes",
            "Payment options",
            "Support System",
            "Checkout",
            "Purchase Theme",
          ],
        },
        {
          title: "NetWorking",
          argoments: [
            "Purchase Theme",
            "Our Benefits",
            "Our Team",
            "Our Service",
            "Other Products",
            "My accounts",
          ],
        },
      ],
      categories: [
          'Economy',
          'Design',
          'Coaching',
          'Business',
          'Medicine',
          'Law',
          'Fitness',
      ]
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/footerContent.scss";
</style>