<script>
  import crazy from './components/Employee.vue'


  export default {
    data() {
      return {

      }
    },
    components: {
      crazy
    },
    methods: {
      crazyName(name) {
        console.log(name);
      },
      crazySalary(name, salary) {
        console.log(name, salary);
      }
    }
  }

</script>

<template>
  <crazy @show="crazyName" @show1="crazySalary" />
</template>


<style scoped>

</style>