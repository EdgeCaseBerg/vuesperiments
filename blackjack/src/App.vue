<template>
  <div id="app" class="container">
    <h1>Black Jack</h1>
    <b-nav tabs fill>
      <b-nav-item active>About</b-nav-item>
      <b-nav-item>New Game</b-nav-item>
    </b-nav>

    <b-row v-for="suit in suits" :key="suit">
      <b-col v-for="value in cardValues" :key="value">
        <Card :value='value' :suit='suit' />
      </b-col>
    </b-row>
  </div>
</template>

<script>
import Card from './components/Card'

export default {
  name: 'App',
  components: {
    Card
  },
  data () {
    return {
      suits: ['hearts', 'spades', 'diamonds', 'clubs'],
      cardValues: ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10', 'Jack', 'Queen', 'King', 'Ace']
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
