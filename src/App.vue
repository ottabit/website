<script setup>
import { RouterLink, RouterView } from 'vue-router'
import logo from "@/assets/logo.png"
import typeface from "@/assets/typeface.png"
import photo from "@/assets/photo.png"

import linkedin from "@/assets/icons/linkedin.png"
import email from "@/assets/icons/email.png"
import github from "@/assets/icons/github.png"

let vh = window.innerHeight * 0.01;

document.documentElement.style.setProperty('--vh',`${vh}px`);
</script>

<template>
    <div class="mx-auto bg-white/50 rounded-xl p-4 flex flex-col justify-around items-center main-container w-full">
      <div class="flex flex-row w-fit items-center justify-center">
        <img alt="Ottabit logo" class="max-w-[120px] min-w-0 w-1/3" :src="logo" />
        <img :src="typeface" alt="Typeface" class="max-w-[250px] min-w-0 w-2/3" />
      </div>
      <div class="flex flex-col items-center">
        <img :src="photo" alt="Profile" class="w-2/3 max-w-[350px] min-w-0" />
      </div>
      <div class="flex flex-col items-center justify-center mt-4 mb-4">
        <p class="text-lg text-center">Andrea Doghetti</p>
        <p class="xs:text-xl lg:text-3xl mt-2 mb-2 text-center">Full Stack Web Developer</p>
      </div>
      <div class="flex flex-row items-center justify-center gap-x-4 mt-4">
        <a href="mailto:andrea@ottabit.com" target="_blank">
          <img :src="email" alt="Email" />
        </a>
        <a href="https://github.com/ottabit" target="_blank">
          <img :src="github" alt="Github" />
        </a>
        <a href="https://linkedin.com/in/ottabit/" target="_blank">
          <img :src="linkedin" alt="Linkedin" />
        </a>
      </div>
    </div>
</template>
