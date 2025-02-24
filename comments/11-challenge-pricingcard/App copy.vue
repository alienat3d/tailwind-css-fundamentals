<!-- ? A challenge to style with the TailwindCSS, so it looks close to this one: https://flowbite.com/blocks/marketing/pricing/ -->
<script setup>
import { useDark } from '@vueuse/core'
import PricingCard from './components/PricingCard.vue'

const isDark = useDark()
</script>
<template>
  <label class="absolute top-5 right-5 cursor-pointer">
    <input v-model="isDark" type="checkbox" class="" /> Dark mode
  </label>
  <h1 class="mt-15 mb-5 text-center text-4xl font-bold">Designed for business teams like yours</h1>
  <h2 class="mb-10 mx-auto text-center w-3xl text-2xl font-light text-gray-700 dark:text-gray-400">
    Here we focus on markets where technology, innovation, and capital can unlock long-term value
    and drive economic growth.
  </h2>
  <div class="p-5 flex flex-wrap justify-center gap-8">
    <PricingCard
      :price="29"
      :features="[
        'Unlimited Access to All Features',
        '24/7 Customer Support',
        'Customizable Dashboard',
        'Advanced Analytics Tools',
        'Integration with Third-Party Services',
        'Secure Data Encryption',
      ]"
      name="Starter"
      description="Best option for personal use & for your next project"
    ></PricingCard>
    <PricingCard
      name="Plus"
      :features="[
        'Multi-User Collaboration Tools',
        'Real-Time Data Backup',
        'Mobile App Access',
        'Custom Branding Options',
        'Automated Reporting System',
      ]"
      :price="50"
      description="Great for small teams and anyone looking to scale"
    ></PricingCard>
    <PricingCard
      name="Enterprise"
      :features="[
        'Priority Feature Updates',
        'Extended Data Storage Capacity',
        'Personalized User Experience',
        'In-Depth Training Materials',
        'Dedicated Account Manager',
      ]"
      :price="150"
      description="Best for large scale uses and extended redistribution rights"
    ></PricingCard>
  </div>
</template>

<style>
body {
  font-family: Inter;
}
</style>
