<script>
  export default {
    data() {
      return {
        hidden: true,
      }
    },
    methods: {
      hide: function () {
        this.hidden = false;
      }
    }
  }
</script>

<template>
  <button class="button" @click="hide">hide</button>
  <div v-if="hidden">
    <p class="crazy">+++</p>
    <p class="crazy">+++</p>
    <p class="crazy">+++</p>
  </div>
</template>

<style scoped>

</style>