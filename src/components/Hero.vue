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
                  Your gateway to experiencing the future of gaming before anyone else. Dive into the worlds of upcoming blockbusters like GTA 6, test their mechanics, and immerse yourself in the action before the official release.
                </p>
              </div>
              <p data-aos="fade-up" data-aos-delay="200">
                <a
                  href="https://t.me/BeTheFirstMarket_bot"
                  target="_blank"
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
    <diu class="wrapper">
      <h5 data-aos="fade-up" data-aos-delay="0">
        Click
        <span
            style="
                      background-color: rgba(64, 123, 255, 0.07);
                      color: #407bff;
                    "
        >here</span
        > if you are still have questions
      </h5>

      <a href="#pricing-section" class="learn-more__btn smoothscroll">
        Learn more
      </a>
    </diu>
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

.wrapper {
  display: flex;
  align-items: center;
  flex-direction: column;
}

.learn-more__btn {
  margin-top: 20px;
  color: white;
  background: rgb(64, 123, 255);
  cursor: pointer;
  border: 1px solid rgb(64, 123, 255);
  border-radius: 50px;
  padding: 10px;
  transition: background 0.3s ease;
  outline: none;

  font-size: 25px;
}

.learn-more__btn:hover {
  color: rgb(64, 123, 255);
  background: white;
}
</style>
