<script setup>
import mainPhoto from "../assets/images/hero.jpg";
import { themeColor } from "../data/items";

const heroHeading = "Want to launch it first, right?";
const buttonSeeFeature = "Went to our telegram shop";
const buttonPricing = "Pricing";
</script>

<template>
  <div class="untree_co-hero" id="home-section">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12">
          <div class="row align-items-center">
            <div
              class="col-lg-7 ml-auto order-lg-2"
              data-aos="fade-right"
              data-aos-delay="400"
            >
              <img :src="mainPhoto" alt="Image" class="img-fluid hero-img" />
            </div>
            <div class="col-lg-5">
              <h1 class="heading" data-aos="fade-up" data-aos-delay="0">
                Want to try it
                <span
                    style="
                      background-color: rgba(64, 123, 255, 0.07);
                      color: #407bff;
                    "
                >first</span
                >, right?
              </h1>
              <div class="excerpt" data-aos="fade-up" data-aos-delay="100">
                <p>
                  We have something interesting for
                  <span
                    style="
                      background-color: rgba(64, 123, 255, 0.07);
                      color: #407bff;
                    "
                    >You!</span
                  >
                  <br/>
                  Far far away, behind the word mountains, far from the
                  countries Vokalia and Consonantia, there live the blind texts.
                  Separated they live in Bookmarksgrove right at the coast
                </p>
              </div>
              <p data-aos="fade-up" data-aos-delay="200">
                <a
                  href="#features-section"
                  class="btn btn-primary smoothscroll"
                  style="margin-right: 5px"
                  :style="[
                    { background: themeColor },
                    { borderColor: themeColor },
                  ]"
                  >{{ buttonSeeFeature }}</a
                >
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.pricing:hover {
  color: #fff !important;
}

.hero-img {
  border-radius: 50px;
}

.btn {
  font-size: 16px;
}

.btn:hover {
  background: white !important;
  color: rgb(64, 123, 255) !important;
}
</style>
