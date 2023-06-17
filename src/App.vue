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
      lightwood() {
        alert('book, horse, pig, zombie');
      },
      herondale() {
        alert('steve, dragon, viazer, skelet')
      }
    }
  }

</script>

<template>
  <crazy @show="lightwood" @show1="herondale" />
</template>


<style scoped>

</style>