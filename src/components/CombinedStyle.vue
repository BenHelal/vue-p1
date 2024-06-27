<template>
  <h2 class="g-1">Another Global Style</h2>
  <h2 class="l-1">Another Local Style</h2>
</template>

<style>
.g-1 {
  background: fuchsia;
  color: aqua;
}
</style>

<style scoped>
.l-1 {
  background: aqua;
  color: fuchsia;
}
</style>
