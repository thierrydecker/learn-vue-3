<template>

  <h2>Binding HTML</h2>

  <!--
  Binding an HTML block to an element
  - Use v-html directive
  -->
  <div>
    <span v-html="name"></span>
    is rendered in bold
  </div>

  <!--
  Vulnerability example
  -->
  <div v-html="hack"></div>

</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      name: '<b>Thierry</b>',
      hack: `<a href="#" onclick="alert('You have been hacked...')">Win a prize!</a>`,
    }
  }
}
</script>

<style>
</style>
