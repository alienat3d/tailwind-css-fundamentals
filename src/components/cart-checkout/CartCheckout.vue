<script setup>
import CartCheckoutColumnLeft from './CartCheckoutColumnLeft.vue'
import CartCheckoutColumnRight from './CartCheckoutColumnRight.vue'
import CartCheckoutShadow from './CartCheckoutShadow.vue'
</script>
<template>
  <div class="relative text-white">
    <div
      class="rounded-2xl overflow-hidden bg-[#323239] border-white border-2 grid grid-cols-9 relative z-10"
    >
      <CartCheckoutColumnLeft />
      <CartCheckoutColumnRight />
    </div>
    <CartCheckoutShadow />
  </div>
</template>
