<script setup>
import { DataProject } from "../data/ProjectData";
</script>

<template>
  <div class="w-full bg-UTAMA h-full pt-14 flex justify-center items-center">
    <div class="container flex flex-col">
      <h2 class="text-white border-b-4 font-bold text-5xl w-fit border-MERAH">
        My Project
      </h2>
      <div class="grid lg:grid-cols-3 gap-6 mt-8 md:grid-cols-2 grid-cols-1">
        <div
          v-for="(item, index) in DataProject"
          :key="index"
          :data-href="`/${item.judul.toLowerCase()}`"
          class="text-white flex flex-col gap-2 px-4 py-4 justify-center items-center rounded-md bg-GRAY01 hover:bg-GRAY02 cursor-pointer"
        >
          <img :src="item.project" class="rounded-md" />
          <p class="font-bold text-lg text-center">{{ item.judul }}</p>
          <p class="text-justify">{{ item.deskripsi }}</p>
          <div class="flex flex-row justify-between w-full items-center">
            <p class="font-normal text-MERAH">{{ item.tech }}</p>
            <div class="flex flex-row gap-2">
              <button>
                <img :src="item.github" class="w-6 h-6" />
              </button>
              <button>
                <img :src="item.demo" class="w-6 h-6" />
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
