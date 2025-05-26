<template>
  <!-- <div v-if="modalValue" class="fixed inset-0 z-50 flex items-center justify-center bg-black bg-opacity-50">
    <div class="bg-white rounded-lg shadow-lg w-96 relative">
      <button @click="close" class="absolute top-2 right-2 text-gray-500 hover:text-gray-700">
        X
      </button>
      <div class="p-6">
        <h2 class="text-xl font-bold mb-4">To jest modal</h2>
        <p class="text-gray-700">{{nameuser}}</p>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
const props = defineProps({
  modalValue: {
    type: Boolean,
    required: true
  },
    nameuser: {
        type: String
    }
})

const emit = defineEmits(['modalValue'])

const close = () => {
  emit('modalValue')
} -->

</script>

<style></style>