<script setup>
import { gritScaleQuestions, gritScaleOptions } from '../data/gritScaleQuestions.js';
const props = defineProps({
  index: Number
})
</script>

<template>
  <h1>{{ gritScaleQuestions[index].question }}</h1>
  <button v-for="option in gritScaleOptions">
    {{ option }}
  </button>
</template>

<style scoped>
h1 {
  text-align: left;
  color: #378CE7;
}

button {
  display: block;
  margin: 10px;
  color: #DFF5FF;
  background-color: #5356FF;
}
</style>
