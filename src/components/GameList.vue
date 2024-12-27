<template>
  <div class="games-list">
    <GameItem
      v-for="item in gamesArray"
      :title="item.title"
      :price="item.price"
      :img="item.img"
      :isComingSoon="item.isComingSoon"
    />
  </div>
</template>

<script setup>
import GameItem from "./GameItem.vue";
import gtaImg from "../assets/images/games/gta6.png";

const gamesArray = [
  {
    title: 'GTA 6',
    img: gtaImg,
    isComingSoon: false,
  },
  {
    title: 'GTA 6',
    img: gtaImg,
    isComingSoon: true,
  },
  {
    title: 'GTA 6',
    img: gtaImg,
    isComingSoon: true,
  },
  {
    title: 'GTA 6',
    img: gtaImg,
    isComingSoon: true,
  },
  {
    title: 'GTA 6',
    img: gtaImg,
    isComingSoon: true,
  },
  {
    title: 'GTA 6',
    img: gtaImg,
    isComingSoon: true,
  }
];
</script>

<style scoped>
.games-list {
  margin-top: 20px;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  max-width: 1000px;
  gap: 20px;
}
</style>
