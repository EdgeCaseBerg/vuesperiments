<template>
  <div id="app" class="container">
    <h1>Black Jack</h1>
    <b-nav tabs fill>
      <b-nav-item active>About</b-nav-item>
      <b-nav-item>New Game</b-nav-item>
    </b-nav>
    <b-spinner label="Loading..."></b-spinner>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
  data () {
    return {
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
