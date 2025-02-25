<!-- ? Здесь, опять же, как и в случае с анимацией меню-гамбургера мы использовали класс "group" на родительском элементе и затем анимировали его дочерние элементы при помощи "group-hover". -->
<template>
  <button class="relative flex items-center gap-2 text-sm font-bold uppercase group">
    <span class="z-10">Continue</span>
    <!-- Здесь у нас полоска укорачивается с дополнительным указанием продолжительности анимации "duration-150". -->
    <span
      class="inline-block w-8 h-[2px] bg-[#EA7C67] group-hover:w-6 transition-all duration-150"
    ></span>
    <!-- Здесь у нас обе полоски до наведения на них лежат в плоскости первой, а при наведении поворачиваются на 45°, образуя стрелку. -->
    <span
      class="absolute right-0 top-[50%] translate-y-[-50%] w-3 h-[2px] bg-[#EA7C67] group-hover:rotate-45 origin-right transition-all duration-150"
    ></span>
    <span
      class="absolute right-0 top-[50%] translate-y-[-50%] w-3 h-[2px] bg-[#EA7C67] group-hover:rotate-[-45deg] origin-right transition-all duration-150"
    ></span>
  </button>
</template>
