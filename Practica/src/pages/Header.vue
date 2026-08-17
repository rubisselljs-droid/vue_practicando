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
  <header class="bg-primario">
    <div class="flex justify-between items-center px-10">
      <div class="border-3">
        <img :src="Logo" alt="" class="w-20" />
      </div>

      <div class="flex items-center space-x-8">
        <a
          href="#"
          class="text-texto hover:text-blue-600 p-5 transition-colors font-semibold"
          >MENU</a
        >
        <a
          href="#"
          class="text-texto hover:text-blue-600 transition-colors font-semibold"
          >EQUIPO</a
        >
        <a
          href="#"
          class="text-texto hover:text-blue-600 transition-colors font-semibold"
          >ESTADOS</a
        >
      </div>
    </div>
  </header>
</template>
