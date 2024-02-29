<script setup>

import VNavigator from "@/components/VNavigator.vue";
import VPoster from "@/components/VPoster.vue";
import VFooter from "@/components/VFooter.vue";
</script>

<template>
  <div style="padding:2rem">
    <VNavigator next="Сөйлесім" current="Тыңдалым" previous="Оқылым"/>
    <VPoster name="Диана" course="" src="https://cdn.dribbble.com/userupload/13107032/file/original-983c1a83a504cc875f535411cbeaacf9.jpg?resize=1200x664"/>
    <div class="overview-description">
      <h1 class="overview-header">
        ТЫҢДАЛЫМ
      </h1>
      <div class="overview-questions">
        <p>Осы сұрақтарға жауап берініз:</p>
        <br>
        <ol>
          <li>
            <div>
              <div>
                <div>
                  <span style="font-weight: bold">
                    Видеоны толық тыңдап шыққан соң кездейсоқ кейіпкерлерге қойылған сұрақтарға өз нұсқаңызбен жауап беріп көріңіз:
                  </span>
                  <ul>
                    <li>Адам құқықтары дегеніміз не?</li>
                    <li>Адамның қандай құқықтары бар?</li>
                  </ul>
                </div>
                <div>
              <span style="font-weight: bold">
                Видео бойынша төмендегі сұрақтарға жауап беріңіз:
              </span>
                  <ul>
                    <li>Адам құқықтарының өзектілігінің видеодағы хронологиясына тоқталыңыз;</li>
                    <li>Адам құқықтарының сақталуына үлес қосқан əлемдік тұлғалар жайында не айтылды?</li>
                    <li>БҰҰ негізгі мақсаты қандай?</li>
                    <li>БҰҰ көрсетуі бойынша адам құқықтары қаншау? Олар?</li>
                    <li>Жалпыға ортақ адам құқықтары қайдан басталады?</li>
                    <li>Адам құқықтары бойынша нақты заң бар болғанымен де неге жер жүзінде олар сақтала бермейді? Видеода бұл мəселе жайлы не айтылды?</li>
                  </ul>
                </div>
              </div>
            </div>
          </li>
          <li>
            <div>
              <span style="font-weight: bold">
                  Видеоны толық тыңдап шығыңыз.
              </span>

              <ul>
                <li>БҰҰ бас кеңсесі қай жерде орналасқан?</li>
                <li>Адам құқықтарының мəртебесі деңгейінің сақталуындағы бұл ұйымның рөлі қандай?</li>
                <li>Ұйымға қанша ел мүше?</li>
                <li>Қазақстан бұл ұйымға қай жылы қабылданды?</li>
                <li>Қазақ тілі қай жылы БҰҰ басқосуында ресми тіл ретінде қолданылған екен?</li>
                <li>Бұл əлемдік ұйым, ал өз елімізде дəл адам құқықтарын қорғайтын қандай ұйымдарды
                  білесіз?</li>
              </ul>
            </div>
          </li>
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