<script>
  export default {
    data() {
      return {
        isValid: true,
        isDisabled: true,
      }
    },
    methods: {

    }
  }
</script>

<template>
  <p :class="{valid: isValid, disable: isDisabled}">steve</p>
</template>

<style scoped>
  p.valid {
    padding: 10px;
    margin: 10px;
    background: #08C;
    color: white;
    font-weight: bold;
    text-decoration: none;
  }
</style>