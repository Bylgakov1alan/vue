<script>
  import crazy from './components/Employee.vue'
  import crazyForm from './components/crazyForm.vue'


  export default {
    data() {
      return {
        crazys: [
          {
            id: 1,
            name: 'ad',
            surn: 'vizer'
          },
          {
            id: 2,
            name: 'steve',
            surn: 'world'
          },
          {
            id: 3,
            name: 'dragon',
            surn: 'kray'
          },
        ],

      }
    },
    components: {
      crazy, crazyForm
    },
    methods: {
      add(name, surn) {
        let id = this.crazys.length + 1;
        this.crazys.push({
          id, name, surn
        });
      }
    }
  }

</script>

<template>
  <crazyForm @add="add" />
</template>


<style scoped>

</style>