<template>
  <div id="app">
    <dome1/>
  </div>
</template>

<script>
import dome1 from './components/dome1'

export default {
  name: 'App',
  components: {
    dome1
  }
}
</script>

<style>
html {
  font-size: 16px;
}
body {
  margin: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#app * {
  /* font-size: 1rem; */
}
</style>
