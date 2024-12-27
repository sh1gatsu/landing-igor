<template>
  <div v-if="isAvailable" class="games-item">
    <img class="games-item__img" :src="props.img"/>

    <h3>{{ props.title }}</h3>

    <a
      class="games-item__btn"
      href="https://t.me/BeTheFirstMarket_bot"
      target="_blank"
    >
      Buy in telegram
    </a>
  </div>

  <div v-else class="games-item-soon">
    <img class="games-item__img-soon" :src="comingSoon"/>
  </div>
</template>

<script setup>
import comingSoon from "../assets/images/games/coming-soon.jpg";
import {computed} from "vue";

const props = defineProps({
  title: String,
  img: String,
  isComingSoon: Boolean,
})

const isAvailable = computed(() => !props.isComingSoon);
</script>

<style scoped>
.games-item {
  display: flex;
  align-items: center;
  flex-direction: column;
  background: white;
  border: 10px solid #ffffff;
  -webkit-box-shadow: 0 15px 30px -5px rgba(0, 0, 0, 0.1);
  box-shadow: 0 15px 30px -5px rgba(0, 0, 0, 0.1);
  border-radius: 15px;
  padding: 20px;
  height: 400px;
  width: 250px;
}

.games-item-soon {
  display: flex;
  align-items: center;
  background: white;
  border: 10px solid #ffffff;
  -webkit-box-shadow: 0 15px 30px -5px rgba(0, 0, 0, 0.1);
  box-shadow: 0 15px 30px -5px rgba(0, 0, 0, 0.1);
  border-radius: 15px;
  padding: 20px;
  height: 400px;
  width: 250px;
}

.games-item__img {
  border: 1px solid black;
  border-radius: 15px;
  height: 200px;
  width: 100%;
  margin-bottom: 20px;
}

.games-item__img-soon {
  height: 200px;
  width: 100%;
}

.games-item__price {
  color: #407bff;
  background-color: rgba(64, 123, 255, 0.07);
}

.games-item__btn {
  color: white;
  background: rgb(64, 123, 255);
  cursor: pointer;
  border: 1px solid rgb(64, 123, 255);
  border-radius: 30px;
  padding: 10px;
  transition: background 0.3s ease;
  margin-top: 15px;
}

.games-item__btn:hover {
  color: rgb(64, 123, 255);
  background: white;
}
</style>