<!-- ? При создании формы обнаружилось, что в строках ввода куча повторяющегося кода, так мы пришли к созданию отдельного компонента для них, где мы отдельно вывели в пропы подпись (название строки ввода) и класс, который мы можем добавлять, чуточку видоизменяя какую-то из строк ввода. -->
<script setup>
const props = defineProps({
  label: String,
  class: String,
})

function slugify(str) {
  return str.toLowerCase().replace(/\s/g, '-')
}
</script>
<script>
export default {
  inheritAttrs: false,
}
</script>
<template>
  <div :class="props.class">
    <input
      class="block focus:border-[#EA7C67] focus:outline-none w-full text-sm font-light tracking-wider bg-transparent border-b border-white"
      v-bind="$attrs"
      :id="slugify(label)"
    />
    <label class="text-xs text-gray-500" :for="slugify(label)">{{ label }}</label>
  </div>
</template>
