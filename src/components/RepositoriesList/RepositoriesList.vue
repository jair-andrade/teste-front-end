<template>
  <div class="list-repositories">
    <div class="card-repositories">
      <h2>Angular-AdminLTE</h2>
      <div class="card-repositories-description">
        <p>
          AngularjsApp Implementation on top of renowned Admin-LTE theme
          (https://github.com/almasaeed2010/AdminLTE) now with many useful directives and features.
        </p>
        <button class="button-fav">
          <img src="@/assets/img/star-fav-icon.png" />
        </button>
      </div>
      <div class="favs-counter">
        <img src="@/assets/img/star-icon.png" />
        <p>200</p>
      </div>
    </div>
    <div class="card-repositories">
      <h2>Angular-AdminLTE</h2>
      <div class="card-repositories-description">
        <p>
          AngularjsApp Implementation on top of renowned Admin-LTE theme
          (https://github.com/almasaeed2010/AdminLTE) now with many useful directives and features.
        </p>
        <button class="button-fav">
          <img src="@/assets/img/star-fav-icon.png" />
        </button>
      </div>
      <div class="favs-counter">
        <img src="@/assets/img/star-icon.png" />
        <p>200</p>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { reactive, toRefs } from 'vue'

const data = reactive({
  dataRef: '' as string
})
const { dataRef } = toRefs(data)
</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: #d9d9d9;
  width: 100%;
  height: 5vh;
}
.header-options > a {
  text-decoration: none;
  margin-left: 10px;
  margin-right: 20px;
  color: #000;
  font-weight: bold;
  font-size: 1.1rem;
  font-family: sans-serif;
}
.list-repositories {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 50px 70px;
}

.favs-counter {
  display: flex;
  align-items: center;
}
.favs-counter img {
  width: 25px;
  margin: 10px 5px;
}
.favs-counter p {
  color: #757575;
  font-size: 1rem;
  font-family: sans-serif;
}

.button-fav {
  cursor: pointer;
  border: none;
  background-color: transparent;
}

.card-repositories {
  flex-direction: column;
  display: flex;
  width: 100%;
  margin: 10px 30px;
  border-bottom: 1px solid #000000;
}
.card-repositories h2 {
  margin: 10px 15px;
  font-family: sans-serif;
}

.card-repositories-description {
  display: flex;
  align-items: center;
}

.card-repositories-description p {
  color: #757575;
  margin: 10px 15px;
  font-size: 1rem;
  font-family: sans-serif;
}
.card-repositories-description img {
  width: 50px;
}

.bottom-options {
  display: flex;
  align-items: center;
  justify-content: center;
}

.button-more {
  cursor: pointer;
  margin: 10px;
  width: 186px;
  height: 51px;
  font-weight: bold;
  font-size: 20px;
  border-radius: 10px;
  font-weight: bold;
  background-color: #fff;
  color: #000;
}
</style>
