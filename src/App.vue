<script>
  export default {
    data() {
      return {
        num: 0,
        res: 0,
        sum: 0,
        num1: 0,
        num2: 0,
      }
    },
    methods: {
      calc: function () {
        this.res = Math.sqrt(this.num);
      },
      summary: function () {
        this.sum = this.num1 + this.num2;
      }
    }
  }
</script>

<template>
  <p class="crazy">{{ res }}</p>
  <input class="text-field__input" v-model="num">
  <button class="button" @click="calc">sqrt</button>
  <br>
  <p class="crazy">{{ sum }}</p>
  <input class="text-field__input" v-model=num1>
  <input class="text-field__input" v-model=num2>
  <button class="button" @click="summary">summary</button>
  <br>

</template>

<style scoped>

</style>