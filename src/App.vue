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

<style lang="stylus">
  #app
    color: red
</style>
