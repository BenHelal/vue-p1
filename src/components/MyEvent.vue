<script setup>
import { ref } from 'vue'
let count = ref(0)

const IncrementCounter = () => count.value++
</script>

<template>
  <h1>Count: {{ count }}</h1>
  <button v-on:click="IncrementCounter">Increment</button>
  <button @:click="count--">Decrement</button>
</template>
