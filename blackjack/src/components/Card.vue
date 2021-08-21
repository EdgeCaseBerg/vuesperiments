<template>
  <div class="card" :class="suitClass">
    <b-container v-if="isFaceDown">
      <p>
        Facedown
      </p>
    </b-container>
    <b-container v-else>
      <b-row>
        <b-col cols="4">{{value}}</b-col>
      </b-row>
      <b-row>
        <b-col offset="2" cols="8">{{suit}}</b-col>
      </b-row>
      <b-row>
        <b-col offset="8" cols="4">{{value}}</b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  props: {
    isFaceDown: Boolean,
    value: String,
    suit: String
  },
  computed: {
    suitClass () {
      if (['hearts', 'diamonds'].indexOf(this.suit) > -1) {
        return 'redsuit'
      } else {
        return 'blacksuit'
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .card {
    vertical-align: bottom;
    height: 90%;
    margin: 0.5em;
    padding: 0.5em;
    outline: 0.25em solid black;
  }
  .redsuit {
    color: red;
  }
  .blacksuit {
    color: black;
  }
</style>
