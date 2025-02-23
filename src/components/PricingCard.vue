<script setup>
defineProps({
  price: { type: Number, default: 0 },
  features: { type: String, required: true },
  name: { type: String, required: true },
  description: { type: String, required: true },
})
</script>
<template>
  <div
    class="flex flex-col items-center basis-96 p-9 text-center border-gray-600 border-1 rounded-lg dark:bg-gray-800"
  >
    <div>
      <h3 class="mb-4 text-3xl font-medium">{{ name }}</h3>
      <p class="mb-9 text-lg font-light text-gray-700 dark:text-gray-400">
        {{ description }}
      </p>
      <div class="mb-9">
        <span class="text-5xl font-bold">${{ price }}</span>
        <span class="ml-3 text-gray-700 dark:text-gray-400">/month</span>
      </div>
      <!-- List -->
      <ul class="pb-5" role="list">
        <li class="mb-5 text-left" v-for="feature in features" :key="feature">
          <!-- Icon -->
          <svg
            class="mr-3 inline-block w-5 h-5 text-green-400"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
              clip-rule="evenodd"
            ></path>
          </svg>
          <span class="text-md font-medium">{{ feature }}</span>
        </li>
      </ul>
    </div>
    <a
      class="block mt-auto w-full p-3.5 bg-teal-600 rounded-lg hover:bg-teal-500 active:bg-teal-700 transition-colors"
      href="#"
      >Get started</a
    >
  </div>
</template>
