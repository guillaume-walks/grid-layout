<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">

    <div class="main-container">
      <Header/>
      <Main />
      <Footer />
    </div>

  </div>
</template>

<script>
import Header from './components/Header'
import Footer from './components/Footer'
import Main from './components/Main'

export default {
  name: 'app',
  components: {
    Header,
    Footer,
    Main
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.main-container{
  display: grid;
  
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
}
.main-container > * {
  border: 1px dashed grey;
}
</style>
