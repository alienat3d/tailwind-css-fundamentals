<!-- ? A challenge to style with the TailwindCSS, so a Checkout page looks close to this one: https://dribbble.com/shots/5990244-Daily-UI-002-Checkout -->
<script setup>
// import { useDark } from '@vueuse/core'
import CartCheckout from './components/cart-checkout/CartCheckout.vue'

// const isDark = useDark()
</script>
<template>
  <label class="absolute bottom-5 right-5 cursor-pointer">
    <input v-model="isDark" type="checkbox" class="" /> Dark mode
  </label>
  <h1 class="mt-15 mb-5 text-center text-4xl font-bold">
    A Checkout Page designed by
    <a href="https://dribbble.com/EnioJ" target="_blank">Enio Jergović</a> & coded by
    <a href="https://zapl.in" target="_blank">Al T</a>.
  </h1>
  <div class="mx-auto mt-15 w-4xl">
    <CartCheckout />
  </div>
</template>

<style>
body {
  font-family: Inter;
}
</style>
