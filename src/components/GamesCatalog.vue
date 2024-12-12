<template>
<div class="games-container" id="pricing-section" data-aos="fade-up" data-aos-delay="100">
  <h1>Games Catalog</h1>

  <GameList />

</div>
</template>

<script setup>

import GameList from "./GameList.vue";
</script>

<style scoped>
.games-container {
  display: flex;
  align-items: center;
  flex-direction: column;
  margin-bottom: 120px;
}
</style>