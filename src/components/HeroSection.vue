<script setup>
import HireMe from "../assets/HireMe.svg";
import Download from "../assets/Download.svg";
import HeroBg from "../assets/HeroBg.svg";
import Me from "../assets/Me.svg";
</script>

<template>
  <div class="w-full lg:h-screen bg-UTAMA flex justify-center items-center">
    <div
      class="container flex lg:flex-row flex-col justify-center items-center"
    >
      <div class="flex flex-col gap-6 lg:w-[60%] w-full">
        <h2 class="text-MERAH flex flex-row gap-2 font-bold text-3xl">
          Hello lm,
          <p class="text-white">Arwin Marinta</p>
        </h2>
        <h1 class="text-white flex flex-row gap-2 text-5xl font-bold">
          Front End
          <p class="text-MERAH">Developer</p>
        </h1>
        <p class="text-white font-normal text-lg">
          A dedicated front-end developer with expertise in creating responsive
          and engaging user interfaces, possessing deep skills, and experience
          in implementing innovative designs to enhance user experience.
        </p>
        <div class="flex flex-row gap-6">
          <button
            class="flex flex-row gap-2 px-4 py-2 font-bold text-MERAH rounded-[4px] border-2 justify-center items-center border-MERAH"
          >
            <img :src="HireMe" alt="Download" />
            <p>Hire Me</p>
          </button>
          <button
            class="flex flex-row bg-MERAH rounded-[4px] text-white justify-center items-center gap-2 px-4 py-2 font-bold"
          >
            <img :src="Download" alt="Download" />
            <p>Download CV</p>
          </button>
        </div>
      </div>
      <div class="md:w-[50%] w-full flex justify-center items-center">
        <img :src="Me" alt="Icon" class="rounded-xl" />
      </div>
    </div>
  </div>
</template>
