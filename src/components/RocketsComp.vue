<template>
  <section id="rockets" class="mx-auto max-w-4xl text-center">
    <p class="my-16 text-2xl font-bold">Our Rockets</p>

    <section class="flex flex-col px-4 sm:flex-row">
      <!-- card one -->
      <section
        class="mx-auto flex w-1/2 flex-col items-center rounded-3xl border border-slate-400 py-4"
      >
        <img
          class="my-3 h-auto w-3/5"
          src="https://acme-rockets.onrender.com/img/rocketman.png"
          alt="explorer"
          loading="lazy"
        />

        <p class="my-2 text-xl font-semibold">Explorer</p>
        <p class="text-slate-400">
          <span class="lg:hidden"
            >Affordable <br />
            Exploration</span
          >
          <span class="hidden lg:block">$</span>
        </p>
      </section>

      <!-- card two -->
      <section
        class="mx-auto my-8 flex w-1/2 flex-col items-center rounded-3xl border border-slate-400 py-4 sm:mx-8 sm:my-0"
      >
        <img
          class="my-3 h-auto w-3/5"
          src="https://acme-rockets.onrender.com/img/rocketride.png"
          alt="adventurer"
          loading="lazy"
        />

        <p class="my-2 text-xl font-semibold">Adventurer</p>
        <p class="text-slate-400">
          <span class="lg:hidden"
            >Best Selling <br />
            Rocket!</span
          >
          <span class="hidden lg:block">$$</span>
        </p>
      </section>

      <!-- card three -->
      <section
        class="mx-auto flex w-1/2 flex-col items-center rounded-3xl border border-slate-400 py-4"
      >
        <img
          class="my-3 h-auto w-3/5"
          src="https://acme-rockets.onrender.com/img/rocketlaunch.png"
          alt="infinity"
        />

        <p class="my-2 text-xl font-semibold">Infinity</p>
        <p class="text-slate-400">
          <span class="lg:hidden"
            >Luxury <br />
            Starship</span
          >
          <span class="hidden lg:block">$$$</span>
        </p>
      </section>
    </section>
  </section>
  <hr class="m-auto my-20 w-1/2 lg:w-1/4" />
</template>

<script setup></script>
