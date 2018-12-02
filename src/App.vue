<template>
  <div id="app">
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
}

.main-container{
  display: grid;
  width: 100vw;
  height: 100vh;
  grid-template-columns: 150px auto 150px;
  grid-template-rows: 100px 1fr 50px;
  grid-gap: 10px;
}
.main-container > * {
  border: 1px dashed grey;
}
</style>
