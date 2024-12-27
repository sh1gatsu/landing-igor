<script setup>
const heading = "Our News";
const subHeading = "Far from the countries Vokalia and Consonantia";
const blogItems = [
  {
    title: "GTA 6 Early Build Now Available",
    name: "James",
    date: "December 2024",
    category: "Digital Service",
    photo: "images/person_1.jpg",
  },
  {
    title: "New Feature Update for CyberPunk 2078 Build",
    name: "James",
    date: "November 2024",
    category: "Digital Service",
    photo: "images/person_2.jpg",
  },
  {
    title: "Partnership Announcement with Indie Game Developers",
    name: "James",
    date: "October 2024",
    category: "Digital Service",
    photo: "images/person_3.jpg",
  },
];
</script>

<template>
  <div class="untree_co-section bg-light">
    <div class="container">
      <div class="row mb-4">
        <div class="col-12 text-center" data-aos="fade-up" data-aos-delay="0">
          <h2 class="heading">{{ heading }}</h2>
        </div>
      </div>
      <div class="row">
        <div
          class="col-md-6 mb-4 mb-lg-0 col-lg-4"
          data-aos="fade-up"
          data-aos-delay="0"
        >
          <div class="news-item">
            <div class="vcard d-flex align-items-center mb-4">
              <div class="post-meta">
                <span>{{ blogItems[0].date }}</span>
              </div>
            </div>
            <div class="news-contents mb-4">
              <h3>
                <a>{{ blogItems[0].title }}</a>
              </h3>
            </div>
          </div>
        </div>
        <div
          class="col-md-6 mb-4 mb-lg-0 col-lg-4"
          data-aos="fade-up"
          data-aos-delay="100"
        >
          <div class="news-item">
            <div class="vcard d-flex align-items-center mb-4">
              <div class="post-meta">
                <span>{{ blogItems[1].date }}</span>
              </div>
            </div>
            <div class="news-contents mb-4">
              <h3>
                <a>{{ blogItems[1].title }}</a>
              </h3>
            </div>
          </div>
        </div>
        <div class="col-md-12 col-lg-4" data-aos="fade-up" data-aos-delay="300">
          <div class="news-item">
            <div class="vcard d-flex align-items-center mb-4">
              <div class="post-meta">
                <span>{{ blogItems[2].date }}</span>
              </div>
            </div>
            <div class="news-contents mb-4">
              <h3>
                <a>{{ blogItems[2].title }}</a>
              </h3>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
