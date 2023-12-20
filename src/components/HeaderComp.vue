<template>
  <header class="w-100 fixed left-0 right-0 top-0 h-14 bg-green-800 text-white">
    <nav
      class="m-auto flex h-14 max-w-5xl items-center justify-between px-3 text-xl font-bold"
    >
      <!-- logo -->
      <a href="#">🚀 Acme Rockets</a>

      <!-- mobile menu icon -->
      <section
        class="cursor-pointer text-2xl sm:hidden"
        @click="toggleMobileMenu"
      >
        &#9776;
      </section>

      <!-- desktop menu -->
      <section class="hidden cursor-pointer text-base font-semibold sm:block">
        <ul class="flex space-x-6">
          <li id="#rockets" class="hover:animate-bounce hover:text-slate-300">
            Our Rockets
          </li>
          <li
            id="#testimonials"
            class="hover:animate-bounce hover:text-slate-300"
          >
            Testimonials
          </li>
          <li id="#contact" class="hover:animate-bounce hover:text-slate-300">
            Contact Us
          </li>
        </ul>
      </section>
    </nav>

    <!-- mobile menu -->
    <section
      v-if="isMobileMenu"
      class="flex h-screen items-center justify-center bg-black py-6 text-center text-3xl sm:hidden"
    >
      <ul class="space-y-12">
        <li id="#" class="hover:animate-bounce hover:text-slate-300">Home</li>
        <li id="#rockets" class="hover:animate-bounce hover:text-slate-300">
          Our Rockets
        </li>
        <li
          id="#testimonials"
          class="hover:animate-bounce hover:text-slate-300"
        >
          Testimonials
        </li>
        <li id="#contact" class="hover:animate-bounce hover:text-slate-300">
          Contact Us
        </li>
        <li id="#legal" class="hover:animate-bounce hover:text-slate-300">
          Legal
        </li>
      </ul>
    </section>
  </header>
</template>

<script setup>
import { ref } from "vue";

const isMobileMenu = ref(false);

const toggleMobileMenu = () => {
  isMobileMenu.value = !isMobileMenu.value;
};
</script>

<style scoped></style>
