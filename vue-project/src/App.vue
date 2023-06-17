<script>
  export default {
    data() {

    },
    methods: {
      show: function () {
        alert(new Date().toLocaleDateString());
      }
    }
  }
</script>

<template>
  <a class="inline-link-1" href="https://www.google.ru/" onclick="event.preventDefault()">Link</a>
  <br>
  <br>
  <button class="button" @click.once="show">click</button>
</template>

<style scoped>

</style>