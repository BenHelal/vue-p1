<script setup>
import { reactive } from 'vue'
let initialState = reactive({ val: { count: 0 }, user: ['wbh', 'Jordan'] })

const changeUser = () => {
  initialState.user[0] = 'wajdi'
  initialState.user[1] = 'ben'
}
</script>

<template>
  <h1>Current cout :{{ initialState.val.count }}</h1>
  <h2>Users: {{ initialState.user }}</h2>

  <button @click="initialState.val.count += 10">Add 10</button>
  <button @click="changeUser">change User</button>
  <button @click="initialState.user.push('helal')">add one more</button>
</template>
