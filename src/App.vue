<template>
  <div id="app">
    <HeaderComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent'

export default {
  name: 'App',
  components: {
    HeaderComponent
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
}
</style>
