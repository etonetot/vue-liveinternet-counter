<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <div>
	<liveinternet-counter />
    </div>
  </div>
</template>

<script>
import LiveinternetCounter from './components/LiveinternetCounter.vue'

export default {
  name: 'App',
  components: {
    LiveinternetCounter
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
