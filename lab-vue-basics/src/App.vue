<template>
  <navbar/>
 <p>this is a mathematical operation 2+2={{2+2}}</p>
 {{ stringAsAFunction() }}
  <footer/>
</template>

<script setup>
import footer from './components/footer.vue'
import navbar from "./components/navbar.vue"
import { Ref } from 'vue';

export default{ //en principio esto me sirve para hacer el stringAsAFunction(). No se como se conectan por eso.
  mounted() {
    return{
      message: "this is a string as a function"
    }
  }
}

//iteration 3


</script>

<style scoped>

</style>
