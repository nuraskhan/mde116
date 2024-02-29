<script setup>
import {defineProps} from 'vue';

const props = defineProps({
  src :String,
  name:String,
  course:String
})
</script>

<template>
  <div>
    <img :src="src" alt="poster" class="poster">
    <div style="justify-content: space-between; width: 100%; display: flex; padding: 5px 10px">
      <div class="madeby">
        <span><img src="../assets/author-2.png" alt="author" class="author"></span>
        <span>{{ name }}</span>
      </div>

      <div>{{ course }}</div>
    </div>
  </div>
</template>

<style scoped>
.poster{
  width:100%;
  border-radius: 8px;
}
.author{
  width: 25px;
  height: 25px;
}
.madeby{
  display: flex;
  gap:10px;
}
</style>