<script setup>
import { themeColor } from "../data/items";
import personPhoto from "../assets/images/person_1.jpg";
import mainPhoto from "../assets/images/service1.jpg";

const service1Heading = "Digital Services";
const service1SubHeading = "Digital";
const service1Quote =
  '"Start building your digital collection today and redefine how you play."';
const personName = "James Anderson";
const designation = "Facebook, Product Lead";
function youtubeVideoUrl() {
  const youtubeVideoId = "FzRH7y3LbQE";
  return `https://www.youtube.com/watch?v=QdBZY2fkU-0&ab_channel=RockstarGames`;
}
</script>
<template>
  <div class="untree_co-section" id="features-section">
    <div class="container">
      <div class="row justify-content-between">
        <div class="col-lg-4">
          <span
            class="caption"
            data-aos="fade-up"
            data-aos-delay="0"
            :style="[{ color: themeColor }]"
            >{{ service1Heading }}</span
          >
          <h3 class="heading mb-4" data-aos="fade-up" data-aos-delay="100">
            {{ service1SubHeading }}
          </h3>
          <div class="mb-4" data-aos="fade-up" data-aos-delay="200">
            <p>
              With
              <span
                  style="
                      background-color: rgba(64, 123, 255, 0.07);
                      color: #407bff;
                    "
              >BeTheFirst</span
              >, you gain instant access to early versions of the hottest upcoming games. We ensure seamless downloads and constant updates to enhance your gaming experience.
            </p>
            <ul class="list-unstyled ul-check primary">
              <li>Access exclusive early builds of trending games</li>
              <li>Be the first to play new levels and features</li>
              <li>Share your gameplay moments with fellow enthusiastsg</li>
            </ul>
          </div>
          <div class="mb-4" data-aos="fade-up" data-aos-delay="300">
            <div class="untree_co-testimonial d-flex">
              <div class="text">
                <blockquote>
                  {{ service1Quote }}
                </blockquote>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-7 video-wrapper" data-aos="fade-up" data-aos-delay="400">
          <a :href="youtubeVideoUrl()" class="btn-video" data-fancybox>
            <span class="wrap-icon-play">
              <svg
                class="bi bi-play-fill"
                width="1em"
                height="1em"
                viewBox="0 0 16 16"
                fill="currentColor"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M11.596 8.697l-6.363 3.692c-.54.313-1.233-.066-1.233-.697V4.308c0-.63.692-1.01 1.233-.696l6.363 3.692a.802.802 0 0 1 0 1.393z"
                />
              </svg>
            </span>
            <img :src="mainPhoto" alt="Image" class="img-fluid img-shadow video-img" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.video-wrapper {
  @media (min-width: 992px) {
    margin-top: 120px
  }
}
</style>