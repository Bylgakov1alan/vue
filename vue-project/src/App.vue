<script>
  export default {
    data() {
      return {
        day: 'Пятница',
      }
    },
    methods: {

    }
  }
</script>

<template>
  <p class="crazy" v-if="day === 'Понедельник'">Понедельник</p>
  <p class="crazy" v-if="day === 'Вторник'">Вторник</p>
  <p class="crazy" v-if="day === 'Среда'">Среда</p>
  <p class="crazy" v-if="day === 'Четверг'">Четверг</p>
  <p class="crazy" v-if="day === 'Пятница'">Пятница</p>
  <p class="crazy" v-if="day === 'Суббота'">Суббота</p>
  <p class="crazy" v-if="day === 'Воскресенье'">Воскресенье</p>
</template>

<style scoped>

</style>