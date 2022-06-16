<template>
  <div id="app">
    <ComponentHeader />
    <button @click.stop="onDestroyClicked">Destroy VM</button>
  </div>
</template>

<script>
import ComponentHeader from './components/ComponentHeader.vue'

export default {
  name: 'App',
  components: {
    ComponentHeader
  },
  methods: {
    onDestroyClicked() {
      this.$destroy()
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
