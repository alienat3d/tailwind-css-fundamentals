<script setup>
import AppGrid from './components/AppGrid.vue'
import { useDark } from '@vueuse/core'

const isDark = useDark()
</script>

<template>
  <label class="absolute top-5 right-5 cursor-pointer">
    <input v-model="isDark" type="checkbox" class="" /> Dark mode
  </label>
  <div class="m-10">
    <AppGrid />
  </div>
</template>

<style></style>
