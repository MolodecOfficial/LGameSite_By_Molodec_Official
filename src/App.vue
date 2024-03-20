<template>
  <Modpacks/>
</template>

<script setup>
import Modpacks from "./components/Modpacks/Modpacks.vue";

let customTitle = document.title;
window.addEventListener("blur", () => {
  document.title = "We are waiting for Your return!"
})
window.addEventListener("focus", () => {
  document.title = customTitle;
})

</script>

<style lang="scss">

</style>