<script setup>
import { SkillData } from "../data/SkillData";
</script>

<template>
  <div class="w-full bg-UTAMA h-full pt-14 flex justify-center items-center">
    <div class="container flex flex-col">
      <h2 class="text-white border-b-4 font-bold text-5xl w-fit border-MERAH">
        Skill~
      </h2>
      <div class="grid lg:grid-cols-5 gap-6 mt-8 md:grid-cols-4 grid-cols-2">
        <div
          v-for="(item, index) in SkillData"
          :key="index"
          :data-href="`/${item.name.toLowerCase()}`"
          class="text-white font-bold rounded-sm flex flex-row gap-2 justify-center items-center border-2 py-2 bg-GRAY01 hover:bg-GRAY02 cursor-pointer"
        >
          <img :src="item.Icon" class="w-[23px] h-[23px]" />
          <p>{{ item.name }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
