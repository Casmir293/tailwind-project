<template>
  <section class="font-mono">
    <!-- header -->
    <header-comp />

    <main>
      <!-- hero -->
      <hero />

      <!-- our rockets -->
      <rockets />
    </main>

    <!-- footer -->
    <footer-comp />
  </section>
</template>

<script setup>
import HeaderComp from "./components/HeaderComp.vue";
import Hero from "./components/HeroComp.vue";
import Rockets from "./components/RocketsComp.vue";
import FooterComp from "./components/FooterComp.vue";
</script>

<style scoped></style>
