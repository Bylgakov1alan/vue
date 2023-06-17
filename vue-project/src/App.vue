<script>
  export default {
    data() {
      return {
        num1: 1,
        num2: 2,
        text: 'alec'
      }
    },
    methods: {
      show: function () {
        let text = this.cape(this.text)
        alert(text);
        // alert(this.num1 + this.num2);
      },
      cape: function (str) {
        return str[0].toUpperCase() + str.slice(1);
      }
    }
  }
</script>

<template>
  <div class="crazy">{{ text }}</div>
  <div class="crazy">{{ num1 + num2 }}</div>
  <button class="button" v-on:mouseover="show">mouse</button>
  <button class="button" @click="show">click</button>
</template>

<style scoped>

</style>