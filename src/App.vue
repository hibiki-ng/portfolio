<template>
  <Navbar/>
  <Home/>
  <About/>
</template>

<script>
import Home from './components/Home.vue'
import Navbar from './components/Navbar.vue'
import About from './components/About.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    About
  }
}
</script>

<style lang="scss">

</style>
