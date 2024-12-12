<template>
<div class="games-container" id="pricing-section">
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
}
</style>