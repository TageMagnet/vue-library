<template>
  <div id="app">
      <router-view/>
  </div>
</template>

<script>
export default {
  data: () => ({
    slideToggle: true
  }),
  computed: {
    Book(){
      return this.$store.state.books
    }
  }
}
</script>

<style lang="scss">
body{margin:0;}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  display: flex;
  max-width: 1420px;
  margin: auto;
}
</style>
