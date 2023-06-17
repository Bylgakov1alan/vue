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
  <button @click="show" class="button">date</button>
</template>

<style scoped>

</style>