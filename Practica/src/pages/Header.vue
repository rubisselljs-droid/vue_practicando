<script setup lang="ts">
import Logo from "../assets/Cerveceros.png";

/**
 * import { ref } from 'vue'
import viteLogo from '../assets/vite.svg'
import heroImg from '../assets/hero.png'
import vueLogo from '../assets/vue.svg'

const count = ref(0)
 */
</script>

<template>
  <header class="bg-primario flex">
    <div class="flex justify-between items-center space-x-2.5">
      <div class="border-3">
        <img :src="Logo" alt="" class="w-20" />
      </div>
      <div class="border-3">
        <a href="">MENU</a>
        <a href="">EQUIPO</a>
        <a href="">ESTADOS</a>
      </div>
    </div>
  </header>
</template>
