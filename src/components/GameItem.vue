<template>
  <div class="games-item">
    <img class="games-item__img" :src="mainPhoto"/>

    <h4>GTA 6</h4>

    <h3 class="games-item__price">600 eur</h3>

    <div class="games-item__btn">Buy in telegram</div>
  </div>
</template>

<script setup>
import mainPhoto from "../assets/images/games/gta6-logo-square.png";
</script>

<style scoped>
.games-item {
  display: flex;
  align-items: center;
  flex-direction: column;
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
  margin-bottom: 10px;
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
}

.games-item__btn:hover {
  color: rgb(64, 123, 255);
  background: white;
}
</style>