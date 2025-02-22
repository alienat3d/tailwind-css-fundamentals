<script setup>
import Flexbox from './components/AppFlexbox.vue'
import { useDark } from '@vueuse/core'

const isDark = useDark()
</script>

<template>
  <label class="absolute top-5 right-5 cursor-pointer">
    <input v-model="isDark" type="checkbox" class="" /> Dark mode
  </label>
  <div class="m-10">
    <Flexbox />
  </div>
</template>

<style></style>
