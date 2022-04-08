<template>
  <div id="app">
    <Header :ojt2title=ojt2title />
    <FirstContent/>
    <SecondContent :movies=movies />
    <ThirdContent/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import FirstContent from './components/FirstContent.vue'
import SecondContent from './components/SecondContent.vue'
import ThirdContent from './components/ThirdContent.vue'
export default {
  name: 'App',
  components: {
    Header, Footer, FirstContent, SecondContent, ThirdContent
  },
  data () {
    return {
      ojt2title: 'Welcome from ojt project 2',
      movies: [
        {
          name: 'English Movie'
        },
        {
          name: 'Myanmar Movie'
        },
        {
          name: 'Korea Movie'
        },
        {
          name: 'Thai Movie'
        },
        {
          name: 'India Movie'
        }
      ]
    }
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
</style>
