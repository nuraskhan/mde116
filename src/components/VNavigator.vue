<script setup>
import {computed, defineProps} from 'vue';

const props = defineProps({
  previous :String,
  next:String,
  current:String
})
let linkprev = computed(()=>{
    if(props.previous === 'Оқылым'){
      return '/reading'
    }else if(props.previous === 'Тыңдалым'){
      return '/listening'
    }else if(props.previous === 'Сөйлесім'){
      return '/speaking'
    }else if(props.previous === 'Жазылым'){
      return '/writing'
    }else{
      return '/'
    }
})
let linknext = computed(()=>{
  if(props.next === 'Оқылым'){
    return '/reading'
  }else if(props.next === 'Тыңдалым'){
    return '/listening'
  }else if(props.next === 'Сөйлесім'){
    return '/speaking'
  }else if(props.next === 'Жазылым'){
    return '/writing'
  }else{
    return '/'
  }
})
</script>

<template>
    <div class="nav-header">
      <div class="nav-logo">MDE-116</div>
      <div class="nav-panels" v-if="previous!=null"> <router-link :to="{path:linkprev}">{{previous}}</router-link> <span><img src="../assets/left.png" alt="" style="width: 10px"></span></div>
      <div class="nav-panels" v-if="next != null"> <router-link :to="{path:linknext}">{{next}}</router-link><span><img src="../assets/right.png" alt="" style="width: 10px;height: 10px"></span></div>
    </div>
  <div class="discover">
    <div class="discover-panel" :class="{und: current=='Шолу'}">
    <router-link to="/">Шолу</router-link></div>
    <div class="discover-panel" :class="{und: current=='Оқылым'}">
      <router-link to="/reading">Оқылым</router-link>
    </div>
    <div class="discover-panel" :class="{und: current=='Тыңдалым'}">
      <router-link to="/listening">Тыңдалым</router-link>
    </div>
    <div class="discover-panel" :class="{und: current=='Сөйлесім'}">
      <router-link to="/speaking">Сөйлесім</router-link>
    </div>
    <div class="discover-panel" :class="{und: current=='Жазылым'}">
      <router-link to="/writing">Жазылым</router-link>
    </div>
  </div>
</template>

<style scoped>
.nav-header{
  min-width:326px;
  display: flex;
  justify-content: space-between;
  border-bottom: 2px solid ;
  padding:20px 10px;
}
.nav-logo{
  font-size: 30px;
  font-family: "American Typewriter";
}
.nav-panels{
  border:1px solid;
  border-radius: 4px;
  padding: 10px 20px;
}
.discover{
  overflow: scroll;
  min-width:326px;
  display: flex;
  padding:20px 0;

}
.discover-panel{
  font-weight: bold;
  cursor: pointer;
  padding:10px 20px;
}
a{
  color: black;
}
a:hover{
  background-color: white;
}
.und{
  border-bottom: 2px solid;
}
</style>