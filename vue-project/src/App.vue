<script>
  export default {
    data() {
      return {
        items: [1, 2, 3, 4, 5],
      }
    },
    methods: {

    }
  }
</script>

<template>
  <div class="crazy" v-for="elem in items">{{ elem }}</div>
  <br>
  <br>
  <div class="crazy" v-for="elem in items">{{ elem*elem }}</div>
  <br>
  <br>
  <ul class="crazy" v-for="elem in items">{{ elem }}</ul>
</template>

<style scoped>

</style>