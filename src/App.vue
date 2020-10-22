<template>
  <div id="app">
    <PdCounter />
  </div>
</template>

<script>
import PdCounter from "@/components/PdCounter"

export default {
  name: 'App',
  components: {
    PdCounter,
  },
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
