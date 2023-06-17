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
        ]
      }
    },
    methods: {
      edit(crazy) {
        crazy.isEdit = true;
      },
      save(crazy) {
        crazy.isEdit = false;
      },
    }
  }
</script>

<template>

  <table class="crazy">
    <tr v-for="crazy in crazys" :key="crazy.id">
      <template v-if="!crazy.isEdit">
        {{ crazy.name }} {{ crazy.salary }} {{ crazy.age }}<button class="button" @click="edit(crazy)">edit</button>
      </template>
      <template v-else>
        <input v-model="crazy.name">
        <input v-model="crazy.salary">
        <input v-model="crazy.age">
        <button class="button" @click="save(crazy)">
          save
        </button>
      </template>
    </tr>
  </table>
</template>

<style scoped>

</style>