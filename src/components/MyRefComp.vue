<script setup>
import { ref } from 'vue'

let count = ref(0)
let username = ref('')
let userList = ref(['Wajdi', 'ben', 'helal'])
let user = ref({name:'wajdi', age:20, location: ['nyc', 'idk'], isMarried: false}) 
</script>

<template>
  <h1>count : {{ count }}</h1>
  <button @click="count--">-</button>
  <button @click="count++">+</button>

  <h1>username : {{ username }}</h1>
  <button @click="username = 'username field'">Add username</button>

  <h1>userList : {{ userList }}</h1>
  <button @click="userList.push('wbh')">add</button>

  <h1>Name: {{ user.name }}</h1>
  <h1>age: {{ user.age }}</h1>
  <h1>location: {{ user.location }}</h1>
  <h1>isMarried: {{ user.isMarried }}</h1>

  <button @click="user.name = 'ben helal'">Change Name</button>
  <button @click="user.age = 29">change Age</button>
  <button @click="user.location = ['earth']">change Age</button>
  <button @click="user.isMarried = true">change Age</button>
</template>