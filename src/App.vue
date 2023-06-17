<script>
  export default {
    data() {
      return {
        crazy: ' ',
        crazys: ' '
      }
    },
    methods: {
      // vm.submit()
    }
  }
</script>

<template>
  <input class="text-field__input" v-model="crazy" v-on:keyup.enter="submit">
  <p>{{ crazy }}</p>
  <br>
  <a href="#" class="inline-link-1" v-on:keyup.ctrl="sub">steve</a>
  <p></p>
</template>

<style scoped>

</style>