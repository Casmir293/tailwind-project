<template>
  <section
    class="m-auto flex h-screen max-w-4xl flex-col items-center justify-center px-3 pt-14 text-center text-slate-400 sm:flex-row-reverse sm:px-5 sm:text-left"
  >
    <img
      ref="hero_image"
      class="h-auto w-2/3"
      src="https://acme-rockets.onrender.com/img/rocketdab.png"
      alt="rocket man"
    />
    <section ref="hero_text">
      <p class="my-5 text-3xl font-bold text-white sm:text-5xl">
        We Boldly Go <span class="text-purple-300">Where No Rocket</span> Has
        Gone Before...
      </p>
      <p>
        We're building rockets for the next century today. From the moon to
        Mars, Jupiter and beyond...
      </p>
      <p class="my-5">Think Acme Rockets.</p>
    </section>
  </section>

  <hr class="m-auto w-1/2 lg:w-1/4" />
</template>

<script setup>
import { ref, onMounted } from "vue";
import { gsap } from "gsap";

const hero_image = ref(null);
const hero_text = ref(null);

onMounted(() => {
  const tl = gsap.timeline();
  tl.from(hero_image.value, { x: "100vw", duration: 1.5 }).from(
    hero_text.value,
    { x: "-100vw", duration: 1.5 },
    "-=1.5",
  );
});
</script>
