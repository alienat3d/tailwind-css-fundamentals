<script setup>
import AppCard from '@/components/AppCard.vue'
</script>

<template>
  <!-- * 1.0 Значение "10" (как и другие) следует умножать на 4, если хотим узнать px, либо на .25, чтобы узнать в rem. -->
  <!-- 1.1 Так у нас добавляются margin со всех сторон, но если нужны margin по горизонтали, то используем "mx", а по вертикали "my". Также и для отдельных сторон: "mt", "mr", "mb", "ml". -->
  <!-- Go to [src\components\AppCard.vue] -->
  <div class="m-10">
    <AppCard />
  </div>
</template>

<style>
body {
  background-color: #48435c;
}
</style>
