<script>
  export default {
    data() {
      return {
        message: '',
        number: '',
      }
    },
    methods: {

    }
  }
</script>

<template>
  <input class="text-field__input" v-model="message">
  <p class="crazy" :style="{textTransform: 'uppercase'}">{{ message }}</p>
  <br>
  <input class="text-field__input" v-model="number">
  <p class="crazy">{{ number*number }}</p>
</template>

<style scoped>

</style>