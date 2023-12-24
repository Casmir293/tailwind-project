<template>
  <footer class="bg-green-800 text-white">
    <section
      class="mx-auto flex max-w-4xl flex-col px-3 py-6 sm:flex-row sm:justify-around sm:px-5"
    >
      <section>
        <p><i>Acme Rocket-Powered Products, Inc.</i></p>
        <p><i>Lagos, NG.</i></p>
        <p>
          <i>Email:</i>
          <a href="mailto:casmir293@gmail.com"><i> casmir293@gmail.com</i></a>
        </p>
        <p>
          <i>Phone:</i>
          <a href="tel:+2348143299602"><i> 08143299602</i></a>
        </p>
      </section>

      <section class="hidden sm:block">
        <ul class="flex flex-col">
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#rockets">Our Rockets</a>
          </li>
          <li class="my-2 hover:animate-bounce hover:text-slate-300">
            <a href="#testimonials">Testimonials</a>
          </li>
          <li class="hover:animate-bounce hover:text-slate-300">
            <a href="#contact">Contact Us</a>
          </li>
        </ul>
      </section>

      <section class="text-right sm:text-left">
        Copyright &copy; {{ currentYear }} <br />
        All Rights Reserved
      </section>
    </section>
  </footer>
</template>

<script setup>
const currentYear = new Date().getFullYear();
</script>

<style lang="scss" scoped></style>
