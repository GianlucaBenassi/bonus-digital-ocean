<template>
  <div id="app" class="position-relative">
    <Header/>
    <Main/>
    <Footer/>
    <Help/>
  </div>
</template>

<script>
import Header from './components/macro/Header.vue';
import Main from './components/macro/Main.vue';
import Footer from './components/macro/Footer.vue';
import Help from './components/commons/Help.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    Help
  }
}
</script>

<style lang="scss">

@import './assets/style/global.scss';

</style>
