<script>
  export default {
    data() {
      return {
        age: 27,
      }
    },
    methods: {

    }
  }
</script>

<template>
  <p class="crazy" v-if="age < 18">Подросток</p>
  <p class="crazy" v-else-if="19 < age && age < 25">Молодой человек</p>
  <p class="crazy" v-else="age > 26">Мужчина</p>
</template>

<style scoped>

</style>