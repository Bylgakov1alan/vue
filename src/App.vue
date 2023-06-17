<script>
  export default {
    data() {
      return {
        crazys: [
          {
            id: 1,
            name: 'vizer',
            salary: 100,
            age: 19,
          },
          {
            id: 2,
            name: 'dragon',
            salary: 200,
            age: 18,
          },
          {
            id: 3,
            name: 'steve',
            salary: 300,
            age: 25,
          },
        ],
      }
    },
    methods: {
      removecrazy: function (id) {
        this.crazys = this.crazys.filter((crazy) => {
          return crazy.id !== id;
        })
      }
    }
  }
</script>

<template>
  <table class="crazy">
    <tr v-for="crazy in crazys" :key="crazy.id"> {{ crazy.name }} {{ crazy.salary }} {{ crazy.age }} <button
        class="button" @click="removecrazy(crazys.id)">remove</button>
    </tr>
  </table>
</template>

<style scoped>

</style>