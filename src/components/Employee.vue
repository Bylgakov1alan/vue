<script>
  export default {
    props: ['name'],
    data() {
      return {

      }
    }
  }
</script>

<template>
  <ul class="styled">
    <li v-for="crazy in name">{{ crazy }}</li>
  </ul>
</template>