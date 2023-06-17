<script>
export default {
    props: ['name', 'surn', 'age'],
    data() {
        return {

        }
    }
}
</script>

<template>
   <p class="crazy">{{ name }}</p>
   <p class="crazy">{{ surn }}</p>
   <p class="crazy">{{ age }}</p>
</template>