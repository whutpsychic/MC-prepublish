<template>
  <main>
    <div class="img-can">
      <img alt="." :src="imgSrc" />
      <div class="text-msk">
        <!-- 原作者 -->
        <!-- <ul class="text-ul">
          <li class="title">作者</li>
          <li>Benimatic</li>
          <li>AtomicBlom</li>
          <li>Drullkus</li>
          <li>Killer_Demon</li>
          <li>Tamaized</li>
          <li>Williewillus</li>
        </ul> -->
        <!-- 标题 -->
        <!-- <div class="title-can">
          <div class="text-can">
            <p class="title">{{ title }}</p>
            <p class="title2">{{ title }}</p>
          </div>
        </div> -->
        <!-- 标题样式2 -->
        <div class="title-can type2">
          <div class="text-can">
            <p class="title">{{ title }}</p>
            <p class="title2">{{ title }}</p>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script setup>
import { ref, unref, onMounted } from 'vue'
import imgSrc from './assets/img.png'

const title = "暮色森林"

onMounted(() => {



})


</script>

<style>
ul.text-ul {
  margin-top: 200px;
  margin-left: 300px;
}

ul.text-ul .title {
  font-size: 17px;
  color: cyan;
  font-weight: bold;
}

ul.text-ul li {
  font-size: 20px;
  color: #fff;
  font-weight: bold;
  margin-bottom: 0.4em;
}

/* ---------------------------------- */
.title-can {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.title-can .text-can {
  width: 100%;
  position: relative;
  font-size: 100px;
  height: 1.5em;
}

/* ---------------------------------- */
.title-can.type2 {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.title-can.type2 .text-can {
  width: 100%;
  position: relative;
  font-size: 100px;
  height: 1.5em;
  display: flex;
  justify-content: center;
}

.title-can.type2 .text-can p.title,
.title-can.type2 .text-can p.title2 {
  width: 3em;
}

.title-can.type2 .text-can p.title {
  top: -30%;
  left: 38%;
}

.title-can.type2 .text-can p.title2 {
  top: calc(-30% - 2px);
  left: calc(38% - 2px);
}

/* ---------------------------------- */

p.title,
p.title2 {
  width: 100%;
  position: absolute;
  font-weight: bold;
  text-align: center;
  letter-spacing: 0.2em;
}

p.title {
  color: #FFD700;
}

p.title2 {
  color: #FF4500;
  top: -2px;
  left: -2px;
}
</style>
