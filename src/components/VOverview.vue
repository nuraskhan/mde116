<script setup>

import VNavigator from "@/components/VNavigator.vue";
import VPoster from "@/components/VPoster.vue";
import VFooter from "@/components/VFooter.vue";
</script>

<template>
  <div style="padding:2rem">
    <VNavigator next="Оқылым" current="Шолу"/>
    <VPoster name="Нұрасхан" course="CS-2" src="https://cdn.dribbble.com/userupload/13141224/file/original-7a7e32f1cc9e89a41407195744f3effa.jpg?resize=1200x664"/>
    <div class="overview-description">
      <h1 class="overview-header">
        АДАМНЫҢ ЖƏНЕ АЗАМАТТЫҢ КОНСТИТУЦИЯЛЫҚ МƏРТЕБЕСІ
      </h1>
      <div class="overview-questions">
        <p>Осы сұрақтарға жауап берініз:</p>
        <br>
        <ul>
          <li>Адам құқығын сіз қалай түсіндірер едіңіз?</li>
          <li>Жеке адам бостандығы шеңберіне қандай ұғымды жатқызасыз?</li>
          <li>Конституциямыздағы басты құндылық адам құқығы мен бостандығы екені белгілі, осы құндылықты қандай мысалдармен сипаттап бере аласыз?</li>
        </ul>
      </div>

    </div>
  </div>
  <VFooter/>
</template>

<style scoped>

.overview-header{
  margin-top: 20px;
  border: 2px solid;
  padding: 10px;
  box-shadow: 1px 1px 1px 1px;
}
.overview-questions{
  padding: 20px;
}
</style>