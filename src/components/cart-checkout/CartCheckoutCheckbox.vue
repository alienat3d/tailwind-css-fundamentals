<!-- ? Для этого видоизменённого чекбокса мы сбросили его дефолтные стили с помощью спец. класса "appearance-none" и дальше стилизовали его по-новой. Обратим внимание на классы "ring", которые создают этот интересный стилистический эффект промежутка между точкой и кольцом вокруг неё при помощи доп. внутреннего кольца цвета фона "ring-offset-[#323239]". -->
<template>
  <label class="flex items-center justify-end mb-10 text-xs text-gray-500 cursor-pointer">
    <input
      type="checkbox"
      class="w-2 h-2 mr-2 rounded-full appearance-none ring-offset-2 ring-offset-[#323239] ring-white ring-1 checked:bg-[#EA7C67]"
    />
    <slot></slot>
  </label>
</template>
