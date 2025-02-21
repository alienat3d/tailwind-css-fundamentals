<!-- 2.2 Также, представим, что у нас есть ссылки, например навигации по сайту и мы хотим сигнализировать пользователю, где он уже был, а где ещё нет. Для этого подойдёт префикс "visited:". Также можно комбинировать с префиксом "focus" и также сделать outline фиолетовым. -->
<template>
  <ul>
    <li>
      <RouterLink to="/" class="visited:text-purple-500 focus:outline-purple-400">Home</RouterLink>
    </li>
  </ul>
</template>
