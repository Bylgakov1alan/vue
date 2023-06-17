<script>
  export default {
    data() {
      return {
        iscrazy: true,
      }
    },
    methods: {

    }
  }
</script>

<template>
  <p class="crazy" v-if="iscrazy">steve</p>
  <p class="crazy" v-else>dragon</p>
</template>

<style scoped>

</style>