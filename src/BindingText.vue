<template>

  <h2>Binding text</h2>

  <!--
  Binding a static text to an HTML element
  -->
  <div>Hello you</div>

  <!--
  Binding a dynamic text to an HTML element
  - Use mustache syntax
  -->
  <div>Hello {{ name }}</div>

  <!--
  Binding a dynamic text to an HTML element
  - Use mustache syntax with multiple elements
  -->
  <div>{{ greet }} {{ name }}</div>

  <!--
  Binding a dynamic text to an HTML element
  - Use v-text directive
  - Inner element is left blank as it will be replaced with the provided data property
  - An error will occur if the inner element is not blank
  -->
  <div v-text="lastName"></div>

</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      name: 'Thierry',
      greet: 'Hello',
      lastName:'Decker'
    }
  }
}
</script>

<style>
</style>
