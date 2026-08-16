

<script setup lang="ts">
import { ref } from "vue"; 
// usamos esto para poder usar la reactividad de vue 
// ref es una funcion que nos permite crear variables reactivas, es decir
//  que cuando cambian su valor, la vista se actualiza automaticamente 
// ES COMO EL RENDER DE REACT, PERO EN VUE 

  let nombre = ref<string>("");
 function Saludar(){
   console.log('hola ' + nombre.value); 
 }

 let numero1 = ref<number>(0);

 function Sumar(){
    numero1.value = numero1.value + 1;
 }

</script>

<template>
   <h1 class="text-white">HOLA MUNDO</h1>


   <h1> Hola mi nombre es : {{ nombre }}</h1>
    
    <!-- v-model conecta el input con la variable nombre, de esta manera cuando el usuario--> 
    <!--escriba en el input, la variable nombre se actualiza automaticamente -->
   <input v-model="nombre" type="text" placeholder="Ingresa tu nombre" />
<h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>

   <button @click="Saludar">Saludar</button>
   <button @click="Sumar">Sumar</button>
   <p>El número es: {{ numero1 }}</p>
</template>