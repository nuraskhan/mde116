<script setup>
import VSpeaking from "@/components/VSpeaking.vue";
import VWriting from "@/components/VWriting.vue";
import VOverview from "@/components/VOverview.vue";

</script>

<template>
  <div class="container">
    <header>

    </header>
    <router-view></router-view>
    <main>
    </main>
  </div>
</template>

<style scoped>
.container{
  min-height: 100vh;
}
header{
  width: 100%;
}

</style>
