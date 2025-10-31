<template>
  <div class="about">
    <h1>My first counter</h1>
    <h2>{{ counter }}</h2>
    <button @click="smanji">-</button>

    <button @click="povecaj">+</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const counter = ref(0)

function smanji() {
  counter.value--
}

function povecaj() {
  counter.value++
}
</script>
