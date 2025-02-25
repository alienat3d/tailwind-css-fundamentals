<!-- ? Здесь мы прибегли к популярной библиотеке "Iconify" для удобного использования иконок. Т.ч. мы импортируем сущность иконок "Icon" из библиотеки, а потом вставляем её в шаблон, при этом название иконки будет передаваться в родительском компоненте через проп "icon", ну и доп. проп "active" будет менять прозрачность, в зависимости от того, активна ли иконка или нет. -->
<script setup>
import { Icon } from '@iconify/vue'
defineProps({
  icon: String,
  active: Boolean,
})
</script>
<template>
  <Icon
    :class="{
      'opacity-100': active,
      'opacity-50': !active,
    }"
    class="hover:drop-shadow-[0_0_6px_#EA7C67] transition-all hover:opacity-100 hover:text-[#fca290]"
    :icon="icon"
  />
</template>
