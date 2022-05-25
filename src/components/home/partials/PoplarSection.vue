<template>
  <!-- Popular section-->
  <section class="page-section bg-light" id="portfolio">
    <div class="container">
      <div class="text-center">
        <h2 class="section-heading text-uppercase">Popular</h2>
        <h3 class="section-subheading text-muted">
          most users are interested in :
        </h3>
      </div>
      <div class="row">
        <div class="col-lg-4 col-sm-6 mb-4" v-for="service in services" :key="service.title">
          <!-- Portfolio item 1-->
          <div class="portfolio-item">
            <a
              class="portfolio-link"
              data-bs-toggle="modal"
              href="#portfolioModal1"
            >
              <div class="portfolio-hover">
                <div class="portfolio-hover-content">
                  <i class="fas fa-plus fa-3x"></i>
                </div>
              </div>
              <img
                class="img-fluid"
                :src="service.image"
                alt="..."
              />
            </a>
            <div class="portfolio-caption">
              <div class="portfolio-caption-heading">{{service.title}}</div>
              <div class="portfolio-caption-subheading text-muted">
                {{ service.description }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import Science from '@/assets/img/portfolio/Science.jpg';
import History from '@/assets/img/portfolio/history.jpg';
import Anime from '@/assets/img/portfolio/anime.jpg';
import Gk from '@/assets/img/portfolio/gk.jpg';
import Sports from '@/assets/img/portfolio/Sports.jpg';
import Food from '@/assets/img/portfolio/food.jpg';

export default {
  name: 'popular-section',
  data() {
    return {
      services: [{
        title: 'Science Quiz',
        description: 'Test Your Basic Science knowledge',
        image: Science,
      },
      {
        title: 'General knowledge',
        description: 'Test Your General knowledge',
        image: Gk,
      },
      {
        title: 'Anime Quiz',
        description: 'Are You An Otaku..? Let\'s See How Much You Know About Anime',
        image: Anime,
      },
      {
        title: 'Sports Quiz',
        description: 'Interested In Sports..? here are some sports quiz for you',
        image: Sports,
      },
      {
        title: 'Food Quiz',
        description: 'Are You A Foodie..? Let\'s Test Your Knowledge About Food',
        image: Food,
      },
      {
        title: 'History quiz',
        description: 'Want to put your history knowledge to the test..?',
        image: History,
      },
      ],
    };
  },
};
</script>
<style lang=""></style>
