<template>
  <div>
    <NuxtRouteAnnouncer />
    <button class="inc" @click="increments">
    Kliknięto {{ count }} 
    </button>

    <button class="inc" @click="ShowHideUsers">
</button>
    <ul v-if="showUsers">
      <li>A</li>
      </ul>
   
  </div>
</template>

<script lang="ts" setup>
const = ref(0)
const showUsers = ref(false)
const increments = () => {
  count.value++
}

const ShowHideUsers = () => {
  showUsers.value = !showUsers.value
}
