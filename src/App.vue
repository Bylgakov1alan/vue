<script>
  export default {
    data() {
      return {
        newcrazy: '',
        crazys: ['steve', 'pig', 'dragon', 'vizer', 'skelet'],
      }
    },
    methods: {
      addcrazy: function () {
        this.crazys.unshift(this.newcrazy);
      }
    }
  }
</script>

<template>
  <ul class="styled">
    <li v-for="(crazy, index) in 
			crazys" :key="index">
      {{ crazy }}
    </li>
  </ul>
  <input class="text-field__input" v-model="newcrazy">
  <br>
  <button class="button" @click="addcrazy">add</button>
</template>

<style scoped>

</style>