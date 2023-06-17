<script>
  export default {
    data() {
      return {
        hidden: true,
        hidden1: false,
      }
    },
  }
</script>

<template>
  <p class="crazy" v-if="hidden">dragon</p>
  <p class="crazy" v-if="!hidden1">steve</p>

</template>

<style scoped>

</style>