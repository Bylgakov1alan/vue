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
            name: 'world',
            surn: 'steve'
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
      change(id, name, surn) {
        this.crazys = this.crazys.map((crazy) => {
          if (crazy.id === id) {
            crazy.name = name;
            crazy.surn = surn;
          }
          return crazy;
        });
      }
    }
  }

</script>

<template>
  <crazy v-for="crazy in crazys" :id="crazy.id" :name="crazy.name" :surn="crazy.surn" :key="crazy.id"
    @change="change" />
</template>


<style scoped>

</style>