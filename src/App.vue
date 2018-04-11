<template>
  <Movies />
  <!-- <div id="app">
    <h1>{{ msg }}</h1>
    <p v-if="isAwesome">Galvanize is AWESOME!!!</p>
    <p v-else>Galvanize is not awesome</p>
    <ul>
      <li v-for="item of items" :key="item">{{ item }}</li>
    </ul>
    <p :class="{hideMe: isHidden}">Hide me</p>
  </div> -->
</template>

<script>
import Movies from './components/Movies.vue'

export default {
  name: 'App',
  components: {
    Movies
  },
  data () {
    return {
      msg: 'Hello Galvanize',
      isAwesome: false,
      items: ['poop', 'butt', 'hello'],
      isHidden: true
    }
  }
}
</script>

<style>
  .hideMe {
    display: none;
  }
</style>
