<script>
  import crazy from './components/Employee.vue'

  export default {
    data() {
      return {
        crazys: [
          {
            id: 1,
            name: 'steve',
            salary: 1000,
            age: 19
          },
          {
            id: 2,
            name: 'dragon',
            salary: 1000,
            age: 18
          },
          {
            id: 3,
            name: 'vizer',
            salary: 3000,
            age: 25
          },
        ],
      }
    },
    components: {
      crazy
    }
  }

</script>

<template>
  <crazy v-for="crazy in crazys" :name="crazy.name" :salary="crazy.salary" :age="crazy.age" :key="crazy.id" />
</template>


<style scoped>

</style>