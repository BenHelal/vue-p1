<template>
  <h1 :class="myClasses['m-class']">Using Module CSS with $ syntax (kabak-case)</h1>
  <h1 :class="myClasses.anotherClass">Using Module CSS with $ syntax (camelCase)</h1>
</template>

<style module="myClasses">
/** kabab-case */
.m-class {
  background: firebrick;
  color: white;
}

.anotherClass {
  background: goldenrod;
  color: aliceblue;
}
</style>
