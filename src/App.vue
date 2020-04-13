<template lang="pug">
  #app
    h1 Banana
    img(alt="Banana" src="./assets/logo.png")
    ApolloExample(msg="Hi there!")
</template>

<script>
  import ApolloExample from "./components/ApolloExample.vue"

  export default {
    name: "App",
    components: {
      ApolloExample,
    },
  }
</script>

<style lang="scss">
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
