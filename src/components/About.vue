<script setup>
import Me from "../assets/Me.svg";
import Ig from "../assets/Ig.svg";
import LinkedIn from "../assets/LinkedIn.svg";
import Github from "../assets/Github.svg";
import Email from "../assets/Email.svg";
</script>

<template>
  <div class="w-full bg-UTAMA flex justify-center items-center">
    <div class="container">
      <div class="bg-GRAY01 flex flex-wrap justify-center py-8 px-16">
        <div class="flex w-[30%] justify-start items-center">
          <img :src="Me" alt="ArwinImage" class="rounded-md" />
        </div>
        <div class="w-[70%] flex flex-col px-2">
          <h1 class="flex flex-row gap-2 font-bold justify-center text-5xl">
            <p class="text-white">About</p>
            <p class="text-MERAH">Me</p>
          </h1>
          <p class="text-white font-normal text-lg mt-9">
            Hi, I'm Arwin Marinta, I'm a student at the Kalimantan Institute of
            Technology, Balikpapan, East Kalimantan. I come from the city of
            Tarakan, North Kalimantan. I have an interest in the field of
            Front-End Web Developer. I am an individual who is passionate and
            committed to the development of attractive and responsive user
            interfaces in the web world.
          </p>
          <h3
            class="text-white font-bold text-2xl mt-5 border-b-[6px] border-MERAH w-fit"
          >
            Sosial Media:
          </h3>
          <div class="flex flex-row gap-4 mt-4">
            <button>
              <img :src="Ig" />
            </button>
            <button>
              <img :src="LinkedIn" />
            </button>
            <button>
              <img :src="Github" />
            </button>
            <button>
              <img :src="Email" />
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
