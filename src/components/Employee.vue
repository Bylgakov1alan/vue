<script>
  export default {
    props: {
      id: Number,
      name: String,
      surn: String,
    },
    emits: ['remove'],
    data() {
      return {

      }
    },
    methods: {
    }
  }
</script>

<template>
  <p class="crazy">{{ name }} {{ surn }}</p>
  <button class="button" @click="$emit('remove', id)">
    remove
  </button>
</template>