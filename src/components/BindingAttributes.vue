<template>

  <h2>Binding HTML</h2>

  <!--
  Binding an attribute to an HTML element
  - Use v-bind syntax
  -->
  <div>
    <p v-bind:id='paragraphId'>A paragraph</p>
  </div>

  <!--
  Binding a boolean attribute to an HTML element
  - Use v-bind syntax
  -->
  <div>
    <button v-bind:disabled='isDisabled'>Enabled ?</button>
  </div>

</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      paragraphId: 'paragraph',
      isDisabled: true,
    }
  }
}

</script>

<style scoped>
</style>