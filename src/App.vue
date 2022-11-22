<template>
  <header>
    <div class="wrapper">
      <TheHeader msg="App Learning App!" />
    </div>
    <RouterView />
  </header>
</template>

<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import TheHeader from "./components/TheHeader.vue";
</script>
