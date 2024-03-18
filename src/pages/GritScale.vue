<script setup>
import Question from '../components/Question.vue';
</script>
<template>
    <div v-for="n in 10">
        <Question :index="n - 1" />
    </div>
</template>