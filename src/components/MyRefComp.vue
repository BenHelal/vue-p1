<script setup>
import { ref } from 'vue'

let count = ref(0)
let username = ref('')
</script>

<template>
  <h1>count : {{ count }}</h1>
  <button @click="count--">-</button>
  <button @click="count++">+</button>

  <h1>username : {{ username }}</h1>
  <button @click="username = 'username field'">Add username</button>
</template>
