<template>
  <div id="app">
    <editor></editor>
    <preview></preview>
  </div>
</template>

<script>
import editor from './components/editor'
import preview from './components/preview'

export default {
  name: 'app',
  components: {
    editor,
    preview
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
