<template>
  <navbar />
  <p>this is a mathematical operation 2+2={{ 2 + 2 }}</p>
  <p>{{ stringAsAFunction() }}</p>
  <button @click="sayHi">salute!</button>
  <p v-if="showMessage">Well Hello!</p>
  <div v-for="post in posts" :key="post.title">
    <h2>{{ post.title }}</h2>
    <p>{{ post.description }}</p>
    <p>{{ post.content }}</p>
  </div>
  <footer />
</template>

<script setup>
import footer from "./components/footer.vue";
import navbar from "./components/navbar.vue";

const posts = $ref([
  {
    title: "This is a title",
    description: "This is a description",
    content: "this is te content",
  },
  {
    title: "This is a title 2",
    description: "This is a description 2",
    content: "this is te content 2",
  },
  {
    title: "This is a title 3",
    description: "This is a description 3",
    content: "this is te content 3",
  },
]);

function sayHello() {
  console.log("hello");
}

sayHello();
</script>

<style scoped></style>
