<template>
  <section
    id="contact"
    class="mx-auto max-w-4xl scroll-mt-32 px-3 pb-14 sm:px-5"
  >
    <p class="mb-5 mt-16 text-center text-2xl font-bold sm:mt-24 lg:text-3xl">
      Contact Us
    </p>

    <section>
      <form action="https://httpbin.org/get" method="get">
        <label for="subject" class="my-4 block">Subject:</label>
        <input
          type="text"
          id="subject"
          name="subject"
          placeholder="Your Subject"
          class="w-full rounded-xl px-3 py-4 text-black"
        />
        <br />
        <label for="message" class="my-4 block">Message:</label>
        <textarea
          id="message"
          name="message"
          rows="12"
          placeholder="Your Message"
          class="w-full rounded-xl px-3 py-4 text-black"
        ></textarea>
        <br />
        <button type="submit" class="mt-4 rounded-xl bg-green-800 px-12 py-3">
          Submit
        </button>
      </form>
    </section>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped></style>
