<script setup lang="ts">
import { ref } from "vue";

const nombre = ref<string>("");

function Eviar() {
  console.log("NOMBRE ENVIADO: " + nombre.value);
}
</script>

<template>
  <header class="bg-black display">
    <nav class="flex justify-between items-center p-4">
      <div class="flex space-x-4">
        <a href="" class="text-white hover:text-gray-300">HOLA </a>
        <a href="" class="text-white hover:text-gray-300">HOLA </a>
      </div>
    </nav>

    <div>
      <h1>MENU</h1>

      <input
        v-model="nombre"
        type="text"
        placeholder="Ingrese su nombre"
        class="bg-white text-yellow"
      />

      <button class="bg-blue-500 text-white p-2 rounded" @click="Eviar">
        Enviar
      </button>
    </div>
  </header>
</template>
