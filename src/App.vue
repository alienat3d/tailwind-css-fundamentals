<script setup>
import { useDark } from '@vueuse/core'
import AppProse from './components/AppProse.vue'

const isDark = useDark()
</script>
<template>
  <label class="absolute top-5 right-5 cursor-pointer">
    <input v-model="isDark" type="checkbox" class="" /> Dark mode
  </label>
  <div class="m-10">
    <AppProse />
  </div>
</template>

<style></style>
