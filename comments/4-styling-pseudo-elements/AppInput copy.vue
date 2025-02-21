<script setup></script>
<!-- * 3.0 Теперь о том как добавлять псевдоэлементы на страницу, например "after". Добавим таким образом "*" после "Username" -->
<template>
  <label class="block mb-3">
    <!-- <span v-if="label" class="block text-2xl text-gray-800">{{ label }}</span> -->
    <span class="block text-2xl text-amber-50 after:content-['*'] after:text-red-500"
      >Username</span
    >
    <!-- 3.1 Также мы можем стилизовать текст-заглушку для строки ввода "placeholder". -->
    <!-- Go to [src\App.vue] -->
    <input
      v-model="_modelValue"
      type="text"
      required="true"
      placeholder="Type In Here Your Username..."
      class="block w-full p-3 border border-gray-400 text-amber-100 rounded-lg focus:outline-lime-600 disabled:opacity-50 invalid:border-red-600 placeholder:italic placeholder:text-gray-400"
    />
  </label>
</template>
