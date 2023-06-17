<script>
  export default {
    data() {
      return {
        text: 'one hargreaves',
      }
    },
    methods: {
      change: function () {
        this.text = 'five hargreaves';
      },
      change2: function () {
        this.text = 'two hargreaves'
      }
    }
  }
</script>

<template>
  <p class="crazy">{{ text }}</p>
  <button class="button" @click="change">text1</button>
  <button class="button" @click="change2">text2</button>
</template>

<style scoped>

</style>