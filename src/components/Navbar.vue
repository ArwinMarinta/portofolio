<script setup>
// Import yang diperlukan dan deklarasi variabel
import Data from "../data/NavData";
</script>

<template>
  <nav
    class="hidden sm:block bg-UTAMA drop-shadow-lg fixed top-0 right-0 left-0"
  >
    <div class="bg-DARKBLUE05">
      <div class="container flex justify-between mx-auto py-4">
        <div class="flex flex-row text-2xl font-bold">
          <p class="text-MERAH font-bold">Wynn</p>
        </div>
        <div
          class="flex flex-row gap-6 font-semibold cursor-pointer text-white"
        >
          <div
            v-for="(item, index) in Data"
            :key="index"
            :href="`/${item.name.toLowerCase()}`"
            class="hover:text-MERAH"
          >
            {{ item.name }}
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
