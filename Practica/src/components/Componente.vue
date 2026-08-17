<script setup lang="ts">
import { ref } from "vue";

const nombre = ref<string>("");

const nombres = [
  "EMir ",
  "Juan",
  "Pedro",
  "Maria",
  "Ana",
  "Luis",
  "Carlos",
  "Sofia",
  "Diego",
  "Valentina",
];

function Eviar() {
  console.log("NOMBRE ENVIADO: " + nombre.value);
}
</script>

<template>
  <header class="display flex justify-around bg-blue-950 items-center">
    <div>
      <img
        src="https://i.pinimg.com/1200x/6c/f8/1c/6cf81c52e105a047f149ad8335f12780.jpg"
        alt="Logo"
        class="h-12 w-12"
      />
    </div>
    <div class="flex space-x-4">
      <a href="" class="text-white hover:text-amber-300">INICIO</a>
      <a href="" class="text-white hover:text-amber-300">NOSOTROS</a>
      <a href="" class="text-white hover:text-amber-300">SERVICIOS</a>
      <a href="" class="text-white hover:text-amber-300">CONTACTO</a>
    </div>
  </header>

  <section class="flex justify-center bg-amber-300 h-screen">
    <!--
    
        <div>
      <h1>INGRESE NOMBRE DEL JUGADOR</h1>

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
    
    -->

    <p
      v-for="nombre in nombres"
      class="flex text-3xl font-bold underline text-white p-2 m-2"
      :key="nombre"
    >
      {{ nombre }}
    </p>
  </section>
</template>
