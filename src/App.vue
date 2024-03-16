<script setup>

import MainPage from "./components/Main/MainPage.vue";
import Section from "./components/Main/Section/Section.vue";

let customTitle = document.title;
window.addEventListener("blur", () => {
  document.title = "We are waiting for your return!";
})
window.addEventListener("focus", () => {
  document.title = customTitle;
})

</script>

<template>
  <MainPage/>
</template>

<style scoped>

</style>
