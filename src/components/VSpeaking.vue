<script setup>

import VNavigator from "@/components/VNavigator.vue";
import VPoster from "@/components/VPoster.vue";
import VFooter from "@/components/VFooter.vue";


</script>

<template>
  <div style="padding:2rem">
    <VNavigator next="Жазылым" current="Сөйлесім" previous="Тыңдалым"/>
    <VPoster name="Ақмарал" course="SDS-2" src="https://cdn.dribbble.com/userupload/13054765/file/original-57be9ba2f8bc5c17db0f0e61902c4e4e.jpg?resize=1200x664"/>
    <div class="overview-description">
      <h1 class="overview-header">
        СӨЙЛЕСІМ
      </h1>
      <div class="overview-questions">
        <p>Адам құқықтары тиісті деңгейде сақталады ма?</p>
        <br>
        <div class="btns">
          <button class="overview-btn" style="background-color: #34e18e">
            Иә, сақталады.
          </button>
          <button class="overview-btn" style="background-color: #cb0303;color: white">
            Жоқ, сақталмайды.
          </button>
        </div>
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
.overview-btn{
  padding: 10px;
  border: 1px solid;
  border-radius: 4px;
  font-size: 25px;
}
.btns{
  width:100%;
  display: flex;
  justify-content: center;
  gap:5px;
}
</style>