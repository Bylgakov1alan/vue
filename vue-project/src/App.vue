<script>
  export default {
    data() {
      return {
        date: '1'
      }
    },
    methods: {
      show: function () {
        let date = this.dayOfWeek(this.date);
        // const dayOfWeekDigit = new Date().getDay();
        // let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
        alert(date);
      },
      dayOfWeek: function (date) {
        let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
        return days[date];
      },
      main: function () {
        const dayOfWeekDigit = new Date().getDay();
        let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
        return dayOfWeekDigit[days]
      },
      // dayOfWeek2: function (date) {
      //   let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
      //   return days[date];
      // }
    }
  }
</script>

<template>
  <!-- <button v-on:mouseover="show">mouse</button> -->
  <button class="button" @click="show">click</button>
  <button class="button" @click="main">click</button>
  {{ dayOfWeekDigit }}
</template>

<style scoped>
  /* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
} */
</style>