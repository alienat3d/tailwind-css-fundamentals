<template>
  <!-- * 8.0 Мы можем успешно миксовать технологии Flexbox & Grid layout. -->
  <!-- ? "!" перед классом означает тоже самое, что и !important в обычном CSS, чтобы удостовериться, что данные классы не перезатрутся в секции "style". Есть также возможность сделать все подобные Tailwind классы со знаком "!", если пропишем в tailwind.config.js "important: true" (может сильно упростить жизнь, если нам нужно прописать TailwindCSS стили в каком-то проекте, использующем высокоприоритетные селекторы стилей). Однако на новых проектах лучше так не делать. -->
  <section class="grid grid-cols-4 gap-2 grid-flow-dense">
    <div></div>
    <div></div>
    <div class="flex items-center justify-around col-span-3">
      <div class="w-16 !min-h-0 h-16 bg-green-300"></div>
      <div class="w-16 !min-h-0 h-16 bg-blue-300"></div>
      <div class="w-16 !min-h-0 h-16 bg-green-300"></div>
      <div class="w-16 !min-h-0 h-16 bg-blue-300"></div>
    </div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
  </section>
</template>
<style scoped>
div {
  background-color: var(--color-gray-400);
  min-height: 100px;
}

div:nth-child(even) {
  background-color: var(--color-gray-600);
}
</style>
