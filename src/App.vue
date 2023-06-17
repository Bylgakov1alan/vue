<script>
  import crazy from './components/Employee.vue'

  export default {
    components: {
      crazy
    }
  }
</script>

<template>
  <crazy :name="['steve', 'vizer', 'dragon', 'zombie', 'pig', 'skelet']" />
</template>


<style scoped>

</style>