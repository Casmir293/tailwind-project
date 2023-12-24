<template>
  <section id="contact">
    <p class="mt-16 text-center text-2xl font-bold sm:mt-24 lg:text-3xl">
      Contact Us
    </p>

    <section>
      <form action="">
        <label for="subject">Subject:</label><br />
        <input
          type="text"
          id="subject"
          name="subject"
          placeholder="Your Subject"
          class="rounded-xl p-3 text-black"
        />
        <br />
        <label for="message">Message:</label> <br />
        <textarea
          id="message"
          name="message"
          placeholder="Your Message"
          class="rounded-xl p-3 text-black"
        >
        </textarea>
        <br />
        <button type="submit" class="mt-2 rounded-xl bg-green-800 px-8 py-2">
          Submit
        </button>
      </form>
    </section>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped></style>
