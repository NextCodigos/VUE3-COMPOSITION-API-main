<script setup>
// alert("HOla desde js")
const name = 'vue dinámico'
const styleColor = "color:blue"
const arrayColores = ["blue", "red", "peru"]
const activo = true
// const activo = false
// const activo = null
// const activo = false
const arryFrutas = ['🍏', '🍇', '🍓', '🥝', '🍒'];

</script>

<template>
  <h1>Hola {{ name.toLocaleUpperCase() }}</h1>

  <h2 v-bind:style="styleColor">Soy AZUL</h2>
  <!-- Cuando cambia el indice cambia el color -->
  <!-- <h2 v-bind:style="`color: ${arrayColores[2]}`">Soy Peru </h2> -->
  <h2 :style="`color: ${arrayColores[2]}`">Soy Peru </h2>

  <h2>
    <!-- Operador ternario -->
    {{ activo ? "Estoy activo" : "Estoy Inactivo" }}
  </h2>

  <h2>{{ arrayColores }}</h2>

  <p v-if="activo === true">
    <span>Icono</span>
    Estoy activo
  </p>

  <p v-else-if="activo === false">Estoy inactivo</p>
  <h2 v-else>Estoy indeciso</h2>

  <h2 v-show="activo">Estoy activo v-show</h2>

  {{ arryFrutas }}
  <!-- FORMA no procedural -->
  <ul>
    <li>{{ arryFrutas[0] }}</li>
    <li>{{ arryFrutas[1] }}</li>
    <li>{{ arryFrutas[2] }}</li>
  </ul>
<!-- v-for igual que arriba pero mejor -->
<ul>
  <li v-for="(fruta,index) in arryFrutas"
  :key="index"
  >{{ index }} - {{ fruta }}
  </li>
</ul>


</template>

<style scoped>
h1 {
  color: red;
}
</style>
