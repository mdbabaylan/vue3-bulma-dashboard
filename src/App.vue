<template>
  <NavBar />
  <div class="container is-fluid">
    Multi-grid tile setup for tablet and desktop. Will be nice!
    All vertical for mobile of course
    Setup the tiles (design on photoshop for consistency, then implement the code, then hook up the public apis to fetch
    the data needed)
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'

export default {
  name: 'App',
  components: {
    NavBar
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
}
</style>
