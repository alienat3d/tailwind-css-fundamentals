<!-- ? A challenge to style with the TailwindCSS, so a navbar component looks close to this one: https://tailwindui.com/components/application-ui/navigation/navbars -->
<script setup>
import { useDark } from '@vueuse/core'
import NavBar from './components/NavBar.vue'

const isDark = useDark()
</script>
<template>
  <NavBar />
  <label class="absolute bottom-5 right-5 cursor-pointer">
    <input v-model="isDark" type="checkbox" class="" /> Dark mode
  </label>
  <h1 class="mt-15 mb-5 text-center text-4xl font-bold">
    A NavBar component inspired by
    <a href="https://tailwindui.com/components/application-ui/navigation/navbars" target="_blank"
      >TailwindUI</a
    >
  </h1>
</template>

<style>
body {
  font-family: Inter;
}
</style>
