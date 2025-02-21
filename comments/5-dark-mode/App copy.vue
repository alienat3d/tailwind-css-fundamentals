<script setup>
// import AppCard from '@/components/AppCard.vue'
import AppButton from '@/components/AppButton.vue'
import AppInput from '@/components/AppInput.vue'
// import TheMainNav from '@/components/TheMainNav.vue'

// 4.1.2 А теперь добавим useDark composable из vueUse, чтобы управлять сменой режимов. useDark будет возвращать булево значение, где true значит, что тёмный режим включён и false — выключен.
import { useDark } from '@vueuse/core'

// 4.1.3 И каждый раз, когда значение isDark переключится на противоположное булево значение, то также и класс "dark" будет добавлен или убран с тега html, переключая режим на сайте.
const isDark = useDark()
</script>

<template>
  <div class="m-10">
    <!-- <AppCard /> -->
    <!-- <TheMainNav /> -->
    <!-- 4.1.4 Ну и, осталось добавить чекбокс для демонстрации. -->
    <input v-model="isDark" type="checkbox" /> Dark mode
    <form action="">
      <label></label>
      <AppInput label="Username" />
      <AppButton>Submit</AppButton>
    </form>
    <p
      class="first-letter:text-5xl first-line:text-2xl selection:bg-green-300 selection:text-black"
    >
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quae facere tempora repudiandae,
      praesentium aliquam enim repellendus vero laudantium totam neque culpa optio quas qui
      consectetur quibusdam! Quasi a officia omnis!
    </p>
    <ul class="mt-5 list-disc marker:text-green-700 marker:text-2xl">
      <li>Vue</li>
      <li>React</li>
      <li>Svelte</li>
      <li>Angular</li>
    </ul>
  </div>
</template>

<style></style>
