<template>
  <!-- 6.1 Затем просто присвоим секции класс "grid", чтобы перевести его элементы в режим "Grid layout". -->
  <!-- 6.2 Теперь разобьём сетку на 4 разных колонки: "grid-cols-4". Также добавим небольшой межколоночник: "gap-2" (также можно выбрать gap только для одной оси, например, "gap-x-2"). -->
  <!-- 6.3 Теперь, чтобы растянуть один из элементов на две колонки: "col-span-2". Также растянем следующий на две строки: "row-span-2". -->
  <!-- 6.4 Ладно, а что, если мы захотим растянуть третий элемент в строке на 3 колонки? У нас образуется дырка сверху, т.к. элементу не хватило колонок на его строке и он "переехал" на следующую. И если в таком случае нам по ТЗ следует заполнить образовавшуюся дыру другими элементами, то мы можем прописать "grid-flow-dense" -->
  <section class="grid grid-cols-4 gap-2 grid-flow-dense">
    <!-- <div class="col-span-2"></div> -->
    <!-- <div class="row-span-2"></div> -->
    <div></div>
    <div></div>
    <div class="col-span-3"></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
  </section>
</template>
<!-- * 6.0 Итак сперва мы стилизуем немного div’ы для наглядности эксперимента. -->
<style scoped>
div {
  background-color: var(--color-gray-400);
  min-height: 100px;
}

div:nth-child(even) {
  background-color: var(--color-gray-600);
}
</style>
