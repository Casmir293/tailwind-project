<template>
  <section class="font-mono">
    <!-- header -->
    <header-comp />

    <main class="w-100 bg-black text-white">
      <!-- hero -->
      <hero />

      <!-- our rockets -->
      <rockets />

      <!-- testimonials -->
      <testimonials />

      <!-- contact -->
      <contact />
    </main>

    <!-- footer -->
    <footer-comp />
  </section>
</template>

<script setup>
import HeaderComp from "./components/HeaderComp.vue";
import Hero from "./components/HeroComp.vue";
import Rockets from "./components/RocketsComp.vue";
import Testimonials from "./components/TestimonialComp.vue";
import Contact from "./components/ContactComp.vue";
import FooterComp from "./components/FooterComp.vue";
</script>

<style>
* {
  scroll-behavior: smooth;
}
</style>
