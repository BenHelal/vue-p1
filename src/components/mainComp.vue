<script setup>
import OptionComp from './optionComp.vue'
const myMessage = 'Yellow World'
const mynumber = 100
const link = 'https://www.google.com'
const logo = 'https://raw.githubusercontent.com/betoma/betoma/master/assets/linkedin.svg'
const altText = 'random logo'

// eslint-disable-next-line no-unused-vars
const anotherLogo = {
  src: 'https://raw.githubusercontent.com/betoma/betoma/master/assets/linkedin.svg',
  alt: 'random logo',
  width: 100,
  height: 100
}
</script>
<!--html-->
<template>
  <div class="container">
    <a :href="link">
      <img id="imgLogo" :src="logo" :alt="altText" />
      <h1 id="h1Main">Hello {{ mynumber }} {{ myMessage }}</h1></a
    >

    <!--Dynamic binding -->
    <img v-bind="anotherLogo" />
    <OptionComp />
  </div>
</template>
<!--css-->

<style>
#h1Main {
  color: red;
}
#imgLogo {
  width: 5%;
}
</style>

<!--js-->
<script>
console.log('hello world')
</script>
