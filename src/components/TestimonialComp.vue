<template>
  <section
    id="testimonials"
    class="testimonials mx-auto max-w-4xl scroll-mt-32 px-3 sm:px-5"
  >
    <p
      class="pin my-6 bg-black py-10 text-center text-2xl font-bold sm:mt-24 lg:text-3xl"
    >
      Testimonials
    </p>

    <!-- first quote -->
    <section class="flex flex-col text-slate-400 sm:text-2xl">
      <blockquote>
        <p>
          <span class="mb-[-50px] block text-7xl text-slate-800">&ldquo;</span>
          <span class="mx-10 block">
            Acme has always been there for me. Their Explorer rocket arrived in
            a wooden crate as expected. Life-long customer! A++ shopping
            experience.</span
          >
          <span class="mt-[-10px] block text-right text-7xl text-slate-800"
            >&rdquo;</span
          >
        </p>
        <br />
        <footer class="mt-[-50px] text-right">
          &mdash;<i>Wile E. Coyote, Genius</i>
        </footer>
      </blockquote>
    </section>

    <!-- second quote -->
    <section class="my-16 flex flex-col text-slate-400 sm:text-2xl">
      <blockquote>
        <p>
          <span class="mb-[-50px] block text-7xl text-slate-800">&ldquo;</span>
          <span class="mx-10 block">
            The Acme Adventurer Rocket has thwarted my Illudium Q-36 Explosive
            Space Modulator on several occassions. This makes me very, very
            angry! Nevertheless, K-9 and I have awarded Acme the Martian
            contract for space exploration rockets based on Acme's quality and
            sturdy designs.</span
          >
          <span class="mt-[-10px] block text-right text-7xl text-slate-800"
            >&rdquo;</span
          >
        </p>
        <br />
        <footer class="mt-[-50px] text-right">
          &mdash;<i>Marvin The Martian & K-9</i>
        </footer>
      </blockquote>
    </section>

    <!-- third quote -->
    <section class="flex flex-col text-slate-400 sm:text-2xl">
      <blockquote>
        <p>
          <span class="mb-[-50px] block text-7xl text-slate-800">&ldquo;</span>
          <span class="mx-10 block">
            I knew I not only wanted — I needed — Acme's Infinity Rocket for my
            mission in space. Acme delivered in one day! Nothing says "<i
              >Take me to your leader</i
            >" like Acme's Infinity Rocket! 💯</span
          >
          <span class="mt-[-10px] block text-right text-7xl text-slate-800"
            >&rdquo;</span
          >
        </p>
        <br />
        <footer class="mt-[-50px] text-right">
          &mdash;<i>Wile E. Coyote, Genius</i>
        </footer>
      </blockquote>
    </section>
  </section>

  <hr class="m-auto my-20 w-1/2 lg:w-1/4" />
</template>

<script setup>
import { onMounted } from "vue";
import gsap from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";

gsap.registerPlugin(ScrollTrigger);

onMounted(() => {
  gsap.from(".testimonials", {
    scrollTrigger: {
      trigger: ".testimonials",
      start: "top +=56px",
      end: "80%",
      scrub: true,
      pin: ".pin",
      pinSpacing: false,
    },
  });
});
</script>
