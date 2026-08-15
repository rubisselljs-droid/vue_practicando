

<script setup lang="ts">
import { ref } from "vue"; // usamos esto para poder usar la reactividad de vue 3

  let nombre = ref<string>("");


</script>

<template>
   <h1>HOLA MUNDO</h1>


   <h1> Hola mi nombre es : {{ nombre }}</h1>


   <input v-model="nombre" type="text" placeholder="Ingresa tu nombre" />
</template>