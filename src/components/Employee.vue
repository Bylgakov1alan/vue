<script>
  export default {
    emits: ['show'],
    data() {
      return {

      }
    },
    methods: {
    }
  }
</script>

<template>
  <button class="button" @click="$emit('show', 'steve')">Name</button>
</template>