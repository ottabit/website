<script setup>
import { RouterLink, RouterView } from 'vue-router'
import logo from "@/assets/logo.png"
import typeface from "@/assets/typeface.png"
import photo from "@/assets/photo.png"

import linkedin from "@/assets/icons/linkedin.png"
import email from "@/assets/icons/email.png"
import github from "@/assets/icons/github.png"
</script>

<template>
  <div class="w-full mx-auto min-h-full">
    <div class="mx-auto bg-white/50 rounded-xl w-full min-h-[93vh] p-4">
      <div class="flex flex-row items-center justify-center">
        <img alt="Ottabit logo" class="min-w-[70px] max-w-[120px] overflow-hidden" :src="logo" />
        <img :src="typeface" alt="Typeface" class="min-w-[180px] max-w-[250px] overflow-hidden" />
      </div>
      <div class="flex flex-col items-center">
        <img :src="photo" alt="Profile" class="min-w-[70px] max-w-[180px] overflow-hidden" />
      </div>
      <div class="flex flex-col items-center justify-center mt-4 mb-4">
        <p class="text-lg text-center">Andrea Doghetti</p>
        <p class="text-xl mt-2 mb-2 text-center">Full Stack Web Developer</p>
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
  </div>
</template>
