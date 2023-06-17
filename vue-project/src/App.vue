<script>
  export default {
    data() {
      return {
        visible: true,
        visible1: false,
      }
    },
  }
</script>

<template>
  <p class="crazy" v-if="visible">dragon</p>
  <p class="crazy" v-if="!visible1">steve</p>

</template>

<style scoped>

</style>