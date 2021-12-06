<template>
  <div id="app">
    <Header/>
    <div id="nav">
      <Menu/>
    </div>
    <router-view/>
    <Footer/>
  </div>
</template>

<script>
import Menu from './components/Menu.vue'
import Footer from './templates/Footer.vue'
import Header from './templates/Header.vue'
export default {
  components: {
    Menu,
    Footer,
    Header
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
