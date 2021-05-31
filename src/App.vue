<template>
  <Navbar/>
  <router-view />
  <Footer/>
</template>

<script>
import Navbar from './components/Navbar'
import Footer from './components/Footer'

export default {
    components : {
      Navbar,
      Footer
    }
}
</script>


<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Mate+SC&display=swap");
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@300&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@600&display=swap');
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  color: #2c3e50;
}
</style>
