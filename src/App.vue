<script>
  export default {
    data() {
      return {
        isDisabled: true,
        isDisabled1: true,
        checked: false,
      }
    },
    methods: {
      toggle: function () {
        this.isDisabled = false;
      },
      toggle1: function () {
        this.isDisabled1 = false;
      },
    }
  }
</script>

<template>
  <input type="text" class="text-field__input" placeholder="stevecrazy" v-bind:disabled="isDisabled">
  <br>
  <button class="button" @click="toggle">btn</button>
  <br>
  <br>
  <br>
  <input type="text" class="text-field__input" placeholder="stevecrazy" v-bind:disabled="isDisabled1">
  <br>
  <input type="checkbox" v-model="checked" @click="toggle1">
  <!-- <button class="button" @click="toggle">btn</button> -->
</template>

<style scoped>

</style>