<script>
  export default {
    data() {
      return {
        crazy: ' ',
      }
    },
    methods: {
      list: function () {

      }
    }
  }
</script>

<template>
  <textarea class="text-field__input" v-model="crazy"></textarea>
  <p class="crazy">{{ crazy }}</p>
  <br>
  <button class="button" @click="list">lists</button>
  <ul>
    <li v-for="craz in crazy">{{ craz }}</li>
  </ul>
</template>

<style scoped>

</style>