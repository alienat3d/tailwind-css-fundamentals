<script setup>
// import AppCard from '@/components/AppCard.vue'
import AppButton from '@/components/AppButton.vue'
import AppInput from '@/components/AppInput.vue'
import TheMainNav from '@/components/TheMainNav.vue'
</script>

<template>
  <div class="m-10">
    <!-- <AppCard /> -->
    <TheMainNav />
    <form action="">
      <label></label>
      <AppInput label="Username" />
      <AppButton>Submit</AppButton>
    </form>
  </div>
</template>

<style>
body {
  background-color: #48435c;
}
</style>
