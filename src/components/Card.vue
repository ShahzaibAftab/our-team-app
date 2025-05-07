<template>
    <div class=" mx-3 w-full max-w-xs bg-white rounded-2xl overflow-hidden shadow-lg p-6 hover:shadow-2xl transition duration-300">
      <!-- Replace image with blue background -->
      <div class="h-50 rounded-xl bg-blue-100 flex items-center justify-center text-white text-3xl font-bold">
      
      </div>
  
      <h2 class="mt-4 text-xl font-bold text-blue-900">{{ price }}</h2>
  
      <p class="text-gray-500 mb-2 text-sm">{{ title }}</p>
      <p class="text-gray-500 mt-2 text-sm">{{ description }}</p>
  
      <!-- Social Icons -->
      <div class="flex justify-start mt-4 space-x-4 text-gray-500">
        <a v-if="twitter" :href="twitter" target="_blank" aria-label="Twitter" class="hover:text-blue-400">
          <i class="fab fa-twitter fa-md"></i>
        </a>
        <a v-if="linkedin" :href="linkedin" target="_blank" aria-label="LinkedIn" class="hover:text-blue-400">
          <i class="fab fa-linkedin-in fa-md"></i>
        </a>
        <a v-if="github" :href="github" target="_blank" aria-label="GitHub" class="hover:text-blue-400">
          <i class="fab fa-github fa-md"></i>
        </a>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Card',
    props: {
      price: {
        type: String,
        default: 'Jane Doe'
      },
      title: {
        type: String,
        default: 'Frontend Developer'
      },
      description: {
        type: String,
        default: 'Description goes here'
      },
    },
  }
  </script>
  
  <style scoped>
  </style>
  