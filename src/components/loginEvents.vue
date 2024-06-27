<script setup>
const submitHandler = (e) => {
  e.preventDefault()
  alert('valid')
}
const showMessage = (message) => alert(message)
</script>

<template>
  <form @:submit="submitHandler">
    <input type="text" placeholder="Please enter your name" />
    <input type="email" placeholder="Please enter your email" />
    <button type="submit">Submit</button>
  </form>
  <button @click="showMessage('this is login message')">Show Msg</button>
</template>
