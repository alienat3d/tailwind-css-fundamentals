<script setup>
import TailwindUILogo from '../assets/img/tailwindui-logo.svg'
import Avatar from '../assets/img/my-avatar.jpeg'
import IconBell from './icons/IconBell.vue'
import IconX from './icons/IconX.vue'

import { ref } from 'vue'
// Создадим реф-переменную, которая будет показывать кликнули ли на аватар или нет. И теперь, когда мы кликаем на аватар, то active сменится на true и будет показано дропдаун-меню.
const active = ref(false)
// Также и для меню "бургер" сделаем реф, который будет показывать активно ли меню или нет.
const mobileMenuActive = ref(false)
</script>

<template>
  <header class="relative flex justify-between items-center px-4 py-3 bg-gray-800">
    <button
      class="burger-menu p-2 w-8.5 min-h-9 bg-gray-700 focus:outline outline-gray-300 rounded sm:hidden"
      @click="mobileMenuActive = !mobileMenuActive"
    >
      <div v-if="mobileMenuActive" class="flex flex-col gap-1.5">
        <span></span>
        <span></span>
        <span></span>
      </div>
      <div v-else>
        <IconX />
      </div>
    </button>
    <img class="ml-12 sm:ml-0 sm:mr-7 w-10 h-10" :src="TailwindUILogo" alt="TailwindUI Logo" />
    <ul
      v-if="mobileMenuActive"
      class="nav-menu absolute top-full left-0 right-0 pb-7 flex flex-col items-center gap-3 bg-gray-800 sm:static sm:flex-row sm:mr-auto sm:pb-0"
    >
      <li class="active">Dashboard</li>
      <li>Team</li>
      <li>Projects</li>
      <li>Calender</li>
    </ul>

    <div class="relative flex">
      <button class="mr-5 text-gray-300 hover:text-white">
        <IconBell />
      </button>
      <button @click="active = !active">
        <img
          class="w-10 h-10 rounded-full ring-gray-300 ring-2 ring-offset-2 ring-offset-gray-800 hover:ring-white"
          :src="Avatar"
          alt="An avatar"
        />
      </button>
      <ul
        class="dropdown-menu z-10 absolute top-full right-0 w-30 bg-gray-50 rounded-md"
        v-if="active"
      >
        <li>Your Profile</li>
        <li>Settings</li>
        <li>Sign Out</li>
      </ul>
    </div>
  </header>
</template>

<style scoped>
@reference "tailwindcss";

.nav-menu {
  @apply pt-8;
  @apply sm:pt-0;
}

.nav-menu li {
  @apply w-[90%];
  @apply rounded-md;
  @apply py-2 px-4;
  @apply text-gray-300;
  @apply text-center;
  @apply sm:w-fit;
}
.nav-menu li:hover {
  @apply bg-gray-700;
  @apply text-white;
}
.nav-menu li:active {
  @apply bg-gray-900;
}
.nav-menu li.active {
  @apply cursor-default;
  @apply text-white;
  @apply bg-gray-900;
}

button,
ul li:hover {
  @apply cursor-pointer;
}

.dropdown-menu li {
  @apply py-1;
  @apply text-black;
}
.dropdown-menu li:hover {
  @apply transition-colors;
  @apply bg-gray-200;
  @apply text-black;
  @apply rounded-none;
}
.dropdown-menu li:first-child:hover {
  @apply rounded-t-sm;
}
.dropdown-menu li:last-child:hover {
  @apply rounded-b-sm;
}

.burger-menu span {
  @apply block;
  @apply h-0.5;
  @apply bg-white;
}
</style>
