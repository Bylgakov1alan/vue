<script>
  import crazy from './components/Employee.vue'

  export default {
    data() {
      return {
        name: 'steve',
        salary: '1000',
        age: '19',
      }
    },
    components: {
      crazy
    }
  }

</script>

<template>
  <crazy :name="name" :salary="salary" :age="age" />
</template>


<style scoped>

</style>