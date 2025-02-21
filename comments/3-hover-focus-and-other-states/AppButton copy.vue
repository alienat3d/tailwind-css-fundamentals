<!-- * 2.0 В TailwindCSS есть специальные префиксы для состояний элементов, будь то "hover:", "active:" или "focus:" которые помогают удобно стилизовать их в соответствующих состояниях и делать анимацию. На примере кнопки укажем изменение цвета при наведении, плавность анимации и смена курсора. -->
<!-- Go to [src\components\AppInput.vue] -->
<template>
  <button
    class="p-3 text-white bg-blue-600 rounded hover:bg-blue-900 transition-colors duration-150 cursor-pointer"
  >
    <slot></slot>
  </button>
</template>
