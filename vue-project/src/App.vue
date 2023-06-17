<script>
  export default {
    data() {
      return {
        isAuth: true,
      }
    },
    methods: {
      toggle: function () {
        this.isAuth = false;
      }
    }
  }
</script>

<template>
  <button class="button" @click="toggle">toggle</button>
  <p class="crazy" v-show="isAuth">steve</p>
</template>

<style scoped>

</style>