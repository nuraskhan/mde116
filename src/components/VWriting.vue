<script setup>

import VNavigator from "@/components/VNavigator.vue";
import VPoster from "@/components/VPoster.vue";
import VFooter from "@/components/VFooter.vue";

import DemoGrid from './VGrid.vue'
import { ref } from 'vue'

const searchQuery = ref('')
const gridColumns = ['Мақал-мәтел', 'Мағынасы']
const gridData = [
  { 'Мақал-мәтел': 'Бала əкеден не не келте туады, не жете туады, не өте туады', Мағынасы: '' },
  { 'Мақал-мәтел': 'Балаңды бес жасқа дейін хандай көтер, Он бес жасқа дейін құлдай жұмса, Он бестен ары онымен досыңдай сырлас', Мағынасы: '' },
  { 'Мақал-мәтел': 'Ұлың өссе үлгілімен ауыл бол', Мағынасы: '' }
]

</script>

<template>
  <div style="padding:2rem">
    <VNavigator current="Жазылым" previous="Сөйлесім"/>
    <VPoster name="Oлжас" course="" src="https://cdn.dribbble.com/userupload/13054746/file/original-3f2cc1357ee90aef336702cd221f1ba3.jpg?resize=1200x664"/>
    <div class="overview-description">
      <h1 class="overview-header">
        ЖАЗЫЛЫМ
      </h1>
      <div class="end">
      </div>
      <DemoGrid
          :data="gridData"
          :columns="gridColumns"
          :filter-key="searchQuery">
      </DemoGrid>
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
.end{
  padding:10px;
  font-weight: bold;
  font-size: 30px;
  justify-content: center;
  width: 100%;
  margin: 0 auto;
  display: flex;
}
.end-text{
  width: fit-content;
}
</style>