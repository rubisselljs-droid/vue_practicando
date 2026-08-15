

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


</script>

<template>
   <h1>HOLA MUNDO</h1>


   <h1> Hola mi nombre es : {{ nombre }}</h1>
    
    <!-- v-model conecta el input con la variable nombre, de esta manera cuando el usuario--> 
    <!--escriba en el input, la variable nombre se actualiza automaticamente -->
   <input v-model="nombre" type="text" placeholder="Ingresa tu nombre" />


   <button @click="Saludar">Saludar</button>
</template>