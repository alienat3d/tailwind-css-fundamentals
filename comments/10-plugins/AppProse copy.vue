<!-- ? https://v3.tailwindcss.com/docs/plugins (дока офиц. плагинов для TailwindCSS) -->
<!-- ? https://github.com/aniftyco/awesome-tailwindcss (настоящий кладезь полезных штук для TailwindCSS и веб-разработки!) -->
<script setup></script>
<!-- * 9.0 Про кастомную конфигурацию видео в папке video. -->
<!-- * 10.0 Подключение плагинов расширяющих функционал TailwindCSS происходит в главном CSS-файле. -->
<!-- Go to [src\assets\main.css] -->
<!-- 10.2 Теперь можно начинать экспериментировать с плагином "typography", который добавляет дополнительные чувствительные типографические стили к контентным блокам, которые приходят из источников вроде CMS-системы и элементы которых не имеют никаких специальных TailwindCSS классов на них. -->
<!-- 10.3 Чтобы плагин "prose" работал также и в тёмном режиме пропишем также "dark:prose-invert". -->
<!-- 10.4 Также мы можем увеличивать или уменьшать текст с помощью "prose-xl (или др. брейкпоинт)". -->
<!-- ? 10.5 Также стоит обратить внимание на ещё один важный Tailwind-плагин "forms", который добавляет сброс стилизации форм, который упрощает стилизацию элементов формы с помощью классов Tailwind: https://github.com/tailwindlabs/tailwindcss-forms -->
<template>
  <article class="prose lg:prose-xl dark:prose-invert">
    <h1 id="heading-1">Garlic bread with cheese: What the science tells us</h1>
    <h2 id="heading-2">Subheading</h2>
    <h3 id="heading-3">Sub-subheading</h3>
    <h4 id="heading-4">Sub-sub-subheading</h4>
    <p>
      For years parents have espoused the health benefits of eating garlic bread with cheese to
      their children, with the food earning such an <em>iconic</em> status in our culture that kids
      will often dress up as warm, cheesy loaf for <strong>Halloween</strong>.
    </p>
    <p>
      But a recent <span>study</span> shows that the celebrated <code>appetizer</code> may be linked
      to a series of rabies cases springing up around the country.
    </p>
    <blockquote>Some genius quote can be here...</blockquote>
    <ol>
      <li>first</li>
      <li>second</li>
      <li>third</li>
    </ol>
  </article>
</template>
