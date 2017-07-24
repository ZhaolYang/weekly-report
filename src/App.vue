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
  *
    box-sizing: border-box
  #app
    display: flex
    min-width: 998px
    height: 100vh
    background-color: #f5f5f5
    padding 20px
</style>
