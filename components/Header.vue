<template>
  <header class="bg-green-600 text-white">
    <div class="container mx-auto px-4 py-4 flex justify-between items-center">
      <div class="text-xl font-bold">Green Allegro</div>

      <div class="flex items-center space-x-2">
        <input type="text" placeholder="Czego szukasz?" class="px-2 py-1 rounded text-black bg-white" />
        <select class="px-2 py-1 rounded text-black bg-white">
          <option>Wszystkie kategorie</option>
        </select>
        <button class="bg-green text-white-600 font-bold px-4 py-1 rounded">SZUKAJ</button>
      </div>

      <nav class="space-x-4">
        <a href="#" class="hover:underline">Home</a>
        <a href="#" class="hover:underline">Kategorie</a>
        <a href="#" class="hover:underline">Promocje</a>
        <a href="#" class="hover:underline">Kontakt</a>
      </nav>
    </div>
  </header>
</template>