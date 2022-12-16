<template>
  <navbar/>
 <p>this is a mathematical operation 2+2={{2+2}}</p>
  <footer/>
</template>

<script setup>
import footer from './components/footer.vue'
import navbar from "./components/navbar.vue"
import { Ref } from 'vue';

const numerical1 = 2568;
const numerical2 = 4775551132;
bunchOfNumbers = numerical1*numerical2;
function(){
  console.log ("bunchOfNumbers");
}

v-if ("bunchOfNumbers">100000000) {
  console.log ("that's a pretty big number.")
}else{
  console.log ("bunchOfNumbers")
};
</script>

<style scoped>

</style>
