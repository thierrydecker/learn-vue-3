<template>

  <h2>Binding Classes</h2>

  <!--
  Binding static classes
  - Use v-bind syntax
  -->
  <h2 class="underlined">Underlined text</h2>

  <!--
  Binding dynamic classes
  - Use v-bind syntax
  -->
  <h2 v-bind:class="status">Status</h2>

  <!--
  Binding both static and dynamic classes
  - Use v-bind syntax
  -->
  <h2 class='underlined' v-bind:class="status">Status</h2>

  <!--
  Binding conditionally
  - Use v-bind syntax
  -->
  <h2 v-bind:class='isPromoted ? "promoted" : "info"'>Status</h2>

  <!--
  Binding multiple classes with an array
  - Use v-bind syntax
  -->
  <h2 v-bind:class='["promoted","info"]'>Status</h2>

  <!--
  Binding multiple classes with an object
  - Use v-bind syntax
  -->
  <h2 v-bind:class="{
        promoted: isPromoted,
        'underlined': isPromoted,
      }">Status</h2>

</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      paragraphId: 'paragraph',
      isDisabled: true,
      status: 'warning',
      isPromoted: true,
    }
  }
}

</script>

<style scoped>

.underlined {
  text-decoration: underline;
}

.danger {
  color: red;
}

.warning {
  color: orange;
}

.info {
  color: green;
}

.promoted {
  font-style: italic;
}

</style>