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
    }
  }

</script>

<template>
  <crazy @show="crazyName" />
</template>


<style scoped>

</style>