<script>
  export default {
    data() {
      return {
        crazys: ['steve', 'dragon', 'vizer'],
      }
    },
    methods: {
      add: function () {
        this.crazys.push('pig');
      },
      del: function () {
        this.crazys.shift();
      },
      del1: function () {
        this.crazys.pop();
      },
      splice: function () {
        this.crazys.splice(2, 1);
      },
      sort: function () {
        this.crazys.sort();
      },
      reverse: function () {
        this.crazys.reverse();
      },
    }
  }
</script>

<template>
  <ul class="styled">
    <li v-for="elem in crazys">{{ elem }}</li>
  </ul>
  <button class="button" @click="add">add crazy</button>
  <br>
  <button class="button" @click="del">delete crazy</button>
  <br>
  <button class="button" @click="del1">delete crazy at the end</button>
  <br>
  <button class="button" @click="splice">delete the penultimate crazy</button>
  <br>
  <button class="button" @click="sort">sort array</button>
  <br>
  <button class="button" @click="reverse">array in reverse order</button>
</template>

<style scoped>

</style>