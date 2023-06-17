<script>
  export default {
    data() {
      return {
        products: [
          {
            id: 1,
            name: 'vizer',
          },
          {
            id: 2,
            name: 'dragon',
          },
          {
            id: 3,
            name: 'steve',
          },
        ]
      }
    },
    methods: {

    }
  }
</script>

<template>
  <p class="crazy" v-for="prod in products" :key='products.id'>{{ prod.name }}</p>
</template>

<style scoped>

</style>