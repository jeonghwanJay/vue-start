<template>
  <form v-on:submit="submitEvent">
    <div>
      <label for="username">ID : </label>
      <input id="username" type="text" v-model="username">
    </div>
    <div>
      <label for="password">PW : </label>
      <input id="password" type="password" v-model="password">
    </div>
    <button type="submit">LOGIN</button>
  </form>
</template>

<script>
export default {
  data: function() {
    return {
      username: '',
      password: '',
    }
  },
  methods: {
    submitEvent: function(event) {
      event.preventDefault();
      console.log(this.username, this.password);
    }
  }
}
</script>

<style>

</style>