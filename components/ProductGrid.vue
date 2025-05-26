<template>
  <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 gap-6 px-4">
    <div v-for="(product, index) in products" :key="index" class="bg-white rounded shadow hover:shadow-lg transition">
      <img :src="product.image" :alt="product.name" class="w-full h-48 object-cover rounded-t" />
      <div class="p-4">
        <h3 class="font-semibold">{{ product.name }}</h3>
        <p class="text-sm text-gray-600" v-if="product.description">{{ product.description }}</p>
        <p class="text-green-600 font-bold mt-2">{{ product.price }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  products: Array
})
</script>