<template>
  <header class="w-100 fixed left-0 right-0 top-0 h-14 bg-green-800 text-white">
    <nav
      class="m-auto flex h-14 max-w-4xl items-center justify-between px-3 text-xl font-bold sm:px-5"
    >
      <!-- logo -->
      <a href="#" class="lg:text-3xl">🚀 Acme Rockets</a>

      <!-- mobile menu icon -->
      <section
        class="transform cursor-pointer text-2xl sm:hidden"
        v-if="!isMobileMenu"
        @click="toggleMobileMenu"
      >
        &#9776;
      </section>

      <section
        class="transform cursor-pointer text-2xl sm:hidden"
        v-else
        @click="toggleMobileMenu"
      >
        &times;
      </section>

      <!-- desktop menu -->
      <section class="hidden cursor-pointer text-base font-semibold sm:block">
        <ul class="flex space-x-6">
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#rockets">Our Rockets</a>
          </li>
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#testimonials">Testimonials</a>
          </li>
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#contact">Contact Us</a>
          </li>
        </ul>
      </section>
    </nav>

    <!-- mobile menu -->
    <transition name="slide">
      <section
        v-if="isMobileMenu"
        class="z-10 flex h-screen items-center justify-center bg-black py-6 text-center text-3xl sm:hidden"
      >
        <ul class="space-y-12">
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#">Home</a>
          </li>
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#rockets">Our Rockets</a>
          </li>
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#testimonials">Testimonials</a>
          </li>
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#contact">Contact Us</a>
          </li>
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#legal">Legal</a>
          </li>
        </ul>
      </section></transition
    >
  </header>
</template>

<script setup>
import { ref } from "vue";

const isMobileMenu = ref(false);

const toggleMobileMenu = () => {
  isMobileMenu.value = !isMobileMenu.value;
};
</script>

<style scoped>
/* mobile menu transition */
.slide-enter-from {
  transform: translateX(100%);
}

.slide-enter-active,
.slide-leave-active {
  transition: transform 0.5s;
}

.slide-leave-to {
  transform: translateX(-100%);
}
</style>
