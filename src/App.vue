<script>
  export default {
    data() {
      return {
        sity: 'Симферополь',
      }
    },
    methods: {

    }
  }
</script>

<template>
  <p class="crazy">В каком городе вы живете?</p>
  <select class="crazy" v-model="sity">
    <option>Симферополь</option>
    <option>Севастополь</option>
    <option>Ялта</option>
  </select>
  <p>{{ sity }}</p>
</template>

<style scoped>

</style>