<template>
  <div class="bg-white text-gray-800">
    <Header />

    <main>
      <section class="bg-green-100 text-center py-16">
        <h1 class="text-4xl font-bold mb-4">Zielone zakupy, lepszy świat</h1>
        <p class="mb-6">Oferujemy produkty eco, lokalne i zrównoważone. Zacznij zmieniać świat już dziś!</p>
        <button class="bg-green-600 hover:bg-green-700 text-white font-bold py-2 px-4 rounded">
          Przeglądaj produkty
        </button>
      </section>

      <section class="py-12">
        <h2 class="text-2xl font-semibold text-center mb-8">Popularne produkty</h2>
        <ProductGrid :products="popularneProdukty" />
      </section>

      <section class="py-12 bg-gray-100">
        <h2 class="text-2xl font-semibold text-center mb-8">Wnętrze w pięknym stylu</h2>
        <ProductGrid :products="wnetrzeProdukty" />
      </section>
    </main>

    <Footer />
  </div>
</template>

<script setup>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import ProductGrid from '@/components/ProductGrid.vue'

const popularneProdukty = [
  {
    name: 'Eko Torba',
    description: 'Torba z materiałów biodegradowalnych',
    price: '39,99 zł',
    image: '/img/zaba.jpg'
  },
  {
    name: 'Kubek Bambusowy',
    description: 'Wielorazowy kubek z bambusa',
    price: '29,90 zł',
    image: '/img/zaba.jpg'
  },
  {
    name: 'Zestaw Zero Waste',
    description: 'Podstawowy zestaw do życia bez odpadów',
    price: '89,00 zł',
    image: '/img/zaba.jpg'
  },
  {
    name: 'Naturalne Świece',
    description: 'Sojowe świece bez sztucznych dodatków',
    price: '59,50 zł',
    image: '/img/zaba.jpg'
  }
]

const wnetrzeProdukty = [
  { name: 'Pufa welurowa', price: '75,00 zł', image: '/img/zaba.jpg' },
  { name: 'Świeczka Bzu', price: '28,99 zł', image: '/img/zaba.jpg' },
  { name: 'Lustro LED', price: '215,99 zł', image: '/img/zaba.jpg' },
  { name: 'Świeczka "Pranie"', price: '33,99 zł', image: '/img/zaba.jpg' },
  { name: 'Stolik nocny', price: '109,00 zł', image: '/img/zaba.jpg' },
  { name: 'Budzik LED', price: '20,89 zł', image: '/img/zaba.jpg' }
]
</script>