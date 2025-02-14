<script setup></script>

<template>
  <!-- 1.2 Итак, сделаем макс. ширину карточки, а также пропишем ей фоновый цвет, тень, padding и скругление краёв. -->
  <div class="max-w-80 bg-amber-50 shadow-lg p-5 rounded-lg">
    <!-- 1.3 Также, к примеру, мы хотим сделать картинку квадратной и укажем ширину и высоту. А также нам нужен класс "object-cover", чтобы изображение увеличилось, а не деформировалось, т.к. оно в оригинале не квадратное и "object-right", чтобы спозиционировать его лучше. -->
    <img
      class="mb-4 rounded-md w-80 h-80 object-cover object-right"
      src="https://placecats.com/700/400"
      alt="cats"
    />
    <!-- 1.4 Также имеет стилизовать заголовок более крупным и тонким шрифтом. Добавим ещё нижнюю линию. -->
    <h4 class="mb-3 pb-3 border-b-1 border-gray-300 font-extralight text-2xl text-center">
      Card Title
    </h4>
    <!-- 1.5 Также мы можем сократить кол-во линий, отображаемых в карточке до 3-ёх с помощью класса "line-clamp-3". -->
    <p class="font-medium line-clamp-3">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique qui in distinctio numquam
      ab quisquam ipsum vero perferendis! Lorem ipsum dolor sit amet.
    </p>
  </div>
</template>
