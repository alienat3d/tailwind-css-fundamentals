<template>
  <!-- * 8.0 Создание адаптивных сайтов в TailwindCSS — одна из звёздных фич, потому, что с ним это делать становится гораздо проще. Достаточно лишь дописать специальный префикс, соответствующий определённым брейкпоинтам вначале. -->
  <!-- 8.1 Итак, нужно помнить, что TailwindCSS по умолчанию Mobile First и поэтому мы считаем, что, например "grid-cols-2" у нас будет от брейкпоинта "sm" и выше. -->
  <!-- 8.2 Если же мы хотим, что стиль действовал лишь в каком-то диапазоне, то можно указать, например, так: "sm:max-md:" -->
  <section class="grid grid-cols-1 gap-2 grid-flow-dense sm:grid-cols-2 md:grid-cols-4">
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div class="sm:max-md:!bg-green-400"></div>
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
