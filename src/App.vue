<script>
  import crazy from './components/Employee.vue'


  export default {
    data() {
      return {
        crazys: [
          {
            id: 1,
            name: 'vizer',
            surn: 'ad'
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
      crazy
    },
    methods: {
      remove(id) {
        this.crazys = this.crazys.filter((crazy) => {
          return crazy.id !== id;
        })
      }
    }
  }

</script>

<template>
  <crazy v-for="crazy in crazys" :id="crazy.id" :name="crazy.name" :surn="crazy.surn" @remove="remove"
    :key="crazy.id" />
</template>


<style scoped>

</style>