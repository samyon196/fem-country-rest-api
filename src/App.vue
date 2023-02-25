<script setup>
import { RouterView } from "vue-router";
import AppBar from "./components/AppBar.vue";
</script>

<template>
  <div class="h-screen w-screen">
    <div class="_topBar box-border relative z-60 bg-white dark:bg-[#2b3743] h-16 w-screen shadow light:shadow-slate-300 flex justify-center">
      <AppBar class="w-5/6" />
    </div>
    <div class="_mainContaienr flex justify-center h-[calc(100%-4rem)] bg-slate-50 dark:bg-[#202d36]">
      <RouterView class="h-full w-5/6" />
    </div>
  </div>
</template>

<style scoped></style>
