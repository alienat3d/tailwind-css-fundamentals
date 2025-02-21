<!-- 2.1 Теперь рассмотрим состояние фокуса, обычно используемое и для кнопок и для строки ввода. Давайте сделаем обрамление строки ввода зелёным, когда фокус на ней и для этого пропишем "focus:outline-lime-600". Таким же образом можно использовать и состояние "disabled", сделаем ему opacity 50%. Также мы можем использовать состояние "invalid" для индикации ошибки проверки строки, подкрасив её красным. -->
<!-- Go to [src\components\TheMainNav.vue] -->
<script setup></script>

<template>
  <label class="block mb-3">
    <span v-if="label" class="block text-2xl text-gray-800">{{ label }}</span>
    <input
      v-model="_modelValue"
      type="text"
      required="true"
      class="block w-full p-3 border border-gray-400 rounded-lg focus:outline-lime-600 disabled:opacity-50 invalid:border-red-600"
    />
  </label>
</template>
