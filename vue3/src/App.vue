<template>
  <main>
    <div class="img-can">
      <img alt="." :src="imgSrc" style="height:100%" />
      <div class="text-msk">
        <!-- 标题样式 -->
        <!-- <div class="title-can multi-lines">
          <div class="text-can">
            <p class="title emphasis">{{ title }}</p>
            <p class="title">{{ title }}</p>
          </div>
          <div class="text-can">
            <p class="title emphasis only1char">&</p>
            <p class="title">&</p>
          </div>
          <div class="text-can">
            <p class="title emphasis">{{ title2 }}</p>
            <p class="title">{{ title2 }}</p>
          </div>
        </div> -->
        <div class="just-two-words">
          <p class="title emphasis">{{ title0 }}</p>
          <p class="title">{{ title0 }}</p>
        </div>
      </div>
    </div>
  </main>
</template>

<script setup>
import { onMounted } from 'vue'
import imgSrc from './assets/img.png'

const title0 = "猛攻"

const title = "一键砍树"
const title2 = "连锁挖掘"

onMounted(() => {

})


</script>

<style>
.text-msk {
  width: 100vw;
  height: 100vh;
  font-size: 150px;
}

.just-two-words {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}

.just-two-words .title {
  position: absolute;
  color: orangered;
  letter-spacing: 1.5em;
  font-weight: bold;
  margin-left: 1.5em;
}

.just-two-words .title.emphasis {
  color: cyan;
  top: calc(50% - 0.64em);
  left: calc(50% - 3.23em);
}

/* ------------------------------------- */
.text-msk .title-can.multi-lines {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-weight: bold;
}

.text-msk .title-can.multi-lines .text-can {
  position: relative;
  margin: 0.2em 50vw;
  height: 1em;
  display: flex;
  justify-content: center;
  white-space: nowrap;
}

.text-msk .title-can.multi-lines .text-can .title {
  position: absolute;
  color: orangered;
  letter-spacing: 0.2em;
}

.text-msk .title-can.multi-lines .text-can .title.emphasis {
  color: cyan;
  top: 2px;
  left: -310px;
}

.text-msk .title-can.multi-lines .text-can .title.emphasis.only1char {
  left: -70px;
}

/* ------------------------------------- */
</style>
