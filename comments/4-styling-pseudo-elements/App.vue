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
    <!-- 3.2 Также может быть иногда полезно стилизовать первую букву в тексте при помощи спец. префикса "first-letter", например, чтобы сделать её ощутимо больше остального текста. Также у нас есть префикс и для стилизации первой линии текста "first-line". -->
    <!-- 3.3 Мы также можем стилизовать и выделение текста с помощью префикса "selection". -->
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
    <!-- 3.4 А также рассмотрим стилизацию ненумерованного списка. По умолчанию нормализация и сброс стилей в TailwindCSS убирает привычные кружочки у ненумерованного списка. Мы можем их вернуть при помощи "list-disc". Но можно пойти дальше и стилизовать этим маркеры дальше, например изменить их цвет на зелёный и увеличить их. Но если хочется получить больше контроля, то может всё таки использовать для этого "before" и уже стилизовать его как угодно. -->
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
