<template>
  <button class="group">
    <!-- ? С помощью классов "group-hover:scale-x-50, transition-all и origin-left" создана интересная анимация меню-гамбургера. Мы специально указали родительскому тегу класс "group", чтобы потом его указать в префиксе "group-hover", т.о. анимация срабатывает на всех элементах с этим префиксом, когда мышка наводится на род. элемент "button.group". "origin-left" нужен, чтобы указать, что анимация должна начинаться с левой стороны. -->
    <span
      class="h-[2px] bg-white w-5 block mb-1 group-hover:scale-x-50 transition-all origin-left"
    ></span>
    <span
      class="h-[2px] bg-white w-3 block mb-1 group-hover:scale-x-150 transition-all origin-left"
    ></span>
    <span
      class="h-[2px] bg-white w-4 block mb-1 group-hover:scale-x-150 transition-all origin-left"
    ></span>
  </button>
</template>
