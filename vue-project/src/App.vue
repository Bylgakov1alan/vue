<script>
  export default {
    data() {
      return {
        visible: true,
        visible1: true,
        visible2: true,
      }
    },
    methods: {
      toggle: function () {
        this.visible = !this.visible;
      },
      toggle1: function () {
        this.visible1 = !this.visible1;
      },
      toggle2: function () {
        this.visible2 = !this.visible2;
      }
    }
  }
</script>

<template>
  <button class="button" @click="toggle">toggle</button>
  <p class="crazy">{{visible ? 'skelet' : 'ton'}}</p>
  <button class="button" @click="toggle1">toggle</button>
  <p class="crazy">{{visible1 ? 'pig' : 'svin'}}</p>
  <button class="button" @click="toggle2">toggle</button>
  <p class="crazy">{{visible2 ? 'steve' : 'luzy'}}</p>
</template>

<style scoped>

</style>