<template>
  <div>
    <h1>{{propsdata}}</h1>
    <button v-on:click="addEvent">add</button>
  </div>
</template>

<script>
export default {
props: ['propsdata'],
methods: {
    addEvent: function() {
        this.$emit('renew')
    }
}
}
</script>

<style>

</style>