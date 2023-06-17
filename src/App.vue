<script>
  export default {
    data() {
      return {
        lang: [],
      }
    },
    methods: {

    }
  }
</script>

<template>
  <div class="crazy">
    <input class="crazy" type="checkbox" v-model="lang" value="js">
    <label>JS</label>
    <br>
    <input class="crazy" type="checkbox" v-model="lang" value="c++">
    <label>C++</label>
    <br>
    <input class="crazy" type="checkbox" v-model="lang" value="java">
    <label>java</label>
    <ol>
      <li v-for="elem in lang">{{ elem }}</li>
    </ol>
  </div>
  <br>
</template>

<style scoped>

</style>