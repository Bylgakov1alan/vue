<script>
  export default {
    data() {
      return {
        arr: ['steve', 'dragon', 'zombie'],
      }
    },
    methods: {

    }
  }
</script>

<template>
  <ul class="crazy" v-for="(elem, key) in arr"> {{ key }} {{ elem }}</ul>
</template>

<style scoped>

</style>