<script>
  export default {
    data() {
      return {
        newcrazy: '',
        crazys: ['steve', 'dragon', 'pig', 'vizer', 'skelet'],
      }
    },
    methods: {
      removecrazy: function (index) {
        this.crazys.splice(index, 1);
      }
    }
  }
</script>

<template>
  <ul class="styled">
    <li v-for="(crazy, index) in 
			crazys" :key="index">
      {{ crazy }}
      <br>
      <button class="button" @click="removecrazy(index)">remove</button>
    </li>
  </ul>
</template>

<style scoped>

</style>