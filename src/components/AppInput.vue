<script setup></script>
<template>
  <label class="block mb-3">
    <span class="block text-2xl after:content-['*'] after:text-red-500">Username</span>
    <input
      v-model="_modelValue"
      type="text"
      required="true"
      placeholder="Type In Here Your Username..."
      class="block w-full p-3 border border-gray-400 rounded-lg focus:outline-lime-600 disabled:opacity-50 invalid:border-red-600 placeholder:italic placeholder:text-gray-400"
    />
  </label>
</template>
