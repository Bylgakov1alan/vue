<script>
  export default {
    data() {
      return {

      }
    },
    methods: {

    }
  }
</script>

<template>
  <p :class="{active: true, error: false}">steve</p>
</template>

<style scoped>
  p.active {
    padding: 10px;
    margin: 10px;
    background: #08C;
    color: white;
    font-weight: bold;
    text-decoration: none;
  }
</style>