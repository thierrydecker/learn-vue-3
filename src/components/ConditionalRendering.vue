<template>

  <h2>Conditional Rendering</h2>

  <!--
  Conditional rendering of an HTML element
  - Use v-if, v-else, v-else-if syntax
  -->
  <h2 v-if="num === 0">The number is zero</h2>
  <h2 v-else-if="num > 0">The number is positive</h2>
  <h2 v-else-if="num < 0">The number is negative</h2>
  <h2 v-else>Not a number</h2>

  <!--
  Conditional rendering of multiple HTML elements
  - Use v-if, v-else, v-else-if syntax
  -->
  <template v-if="display">
    <h2>Thierry</h2>
    <h2>DECKER</h2>
    <h2>Cethun</h2>
  </template>


  <!--
  Conditional rendering of multiple HTML elements
  - Use v-show syntax
  -->
  <div v-show="display">
    <h2>Thierry</h2>
    <h2>DECKER</h2>
    <h2>Cethun</h2>
  </div>

</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      num: 1,
      display: false,
    }
  }
}

</script>

<style scoped>
</style>