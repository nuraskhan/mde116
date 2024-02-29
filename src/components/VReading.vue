<script setup>

import VNavigator from "@/components/VNavigator.vue";
import VPoster from "@/components/VPoster.vue";
import VFooter from "@/components/VFooter.vue";
</script>

<template>
  <div style="padding:2rem">
    <VNavigator next="Тыңдалым" current="Оқылым" previous="Шолу"/>
    <VPoster name="Аружан" course="CS-2" src="https://cdn.dribbble.com/userupload/13131060/file/original-54abf604c34c347440f19cc4b987525b.jpg?resize=1200x664"/>
    <div class="overview-description">
      <h1 class="overview-header">
        ОҚЫЛЫМ
      </h1>
      <div class="overview-questions">
        <p>Осы сұрақтарға жауап берініз:</p>
        <br>
        <ol>
          <li>Халқының құқығын, бостандығын қорғау жолында тағы қандай зиялы қауымның заңдарын білесіз?</li>
          <li>Абай Құнанбайұлының заң баптарына толығырақ тоқталып өтіңіз.</li>
          <li>Əр тұлға адамзат құқықтарының дұрыс сақталуы жолында заң білгеннен басқа тағы
            қандай үлес қоса алады?</li>
          <li>Тəуелсіз елдің егемен жастарының сипаты қандай болуы керек?</li>
          <li>Адамның жəне азаматтың конституциялық мəртебесі жайлы не білесіз?</li>
        </ol>
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