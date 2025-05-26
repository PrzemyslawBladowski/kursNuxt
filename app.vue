<template>
  <button @click="emitModalShow" class="px-4 py-2 bg-blue-500 text-white hover:bg-blue-600">Otworz
    modal</button>

  <Modal @modalValue="emitModalShow" :modalValue="showModal" :nameuser="'Przemek'"/>
</template>
<script setup>
const showModal = ref(false)

const emitModalShow = () => {
  showModal.value = !showModal.value
  console.log(showModal.value)
}
</script>