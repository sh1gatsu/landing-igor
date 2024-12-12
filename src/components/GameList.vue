<template>
  <div class="games-list">
    <GameItem />
    <GameItem />
    <GameItem />
    <GameItem />
    <GameItem />
    <GameItem />
  </div>
</template>

<script setup>
import GameItem from "./GameItem.vue";
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
