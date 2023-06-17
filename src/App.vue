<script>
  export default {
    data() {
      return {
        cssClass: 'craz',
      }
    },
    methods: {

    }
  }
</script>

<template>
  <p :class="cssClass">crazy</p>
</template>

<style scoped>
  .craz {
    padding: 10px;
    margin: 10px;
    background: #08C;
    color: white;
    font-weight: bold;
    text-decoration: none;
  }
</style>