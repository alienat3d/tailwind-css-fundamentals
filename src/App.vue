<script setup>
// import AppCard from '@/components/AppCard.vue'
import AppButton from '@/components/AppButton.vue'
import AppInput from '@/components/AppInput.vue'
// import TheMainNav from '@/components/TheMainNav.vue'
</script>

<template>
  <div class="m-10">
    <!-- <AppCard /> -->
    <!-- <TheMainNav /> -->
    <form action="">
      <label></label>
      <AppInput label="Username" />
      <AppButton>Submit</AppButton>
    </form>
    <p
      class="first-letter:text-5xl first-line:text-2xl selection:bg-green-300 selection:text-black text-amber-50"
    >
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quae facere tempora repudiandae,
      praesentium aliquam enim repellendus vero laudantium totam neque culpa optio quas qui
      consectetur quibusdam! Quasi a officia omnis!
    </p>
    <ul class="mt-5 text-amber-50 list-disc marker:text-green-700 marker:text-2xl">
      <li>Vue</li>
      <li>React</li>
      <li>Svelte</li>
      <li>Angular</li>
    </ul>
  </div>
</template>

<style>
body {
  background-color: #48435c;
}
</style>
