<script>
  export default {
    data() {
      return {
        visible: true,
        visible2: true,
        visible3: true,
      }
    },
    methods: {
      toggle: function () {
        this.visible = !this.visible;
      },
      toggle2: function () {
        this.visible2 = !this.visible2;
      },
      toggle3: function () {
        this.visible3 = !this.visible3;
      }
    }
  }
</script>

<template>
  <button class="button" @click="toggle">1</button>
  <p class="crazy" v-if="visible">vizer</p>
  <button class="button" @click="toggle2">2</button>
  <p class="crazy" v-if="visible2">zombie</p>
  <button class="button" @click="toggle3">3</button>
  <p class="crazy" v-if="visible3">steve</p>
</template>

<style scoped>

</style>