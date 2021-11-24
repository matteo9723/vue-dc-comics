<template>
  <div id="app">
    <Header/>
    <MainTop/>
    <MainBottom/>
    <FooterTop/>
    <FooterBottom/>

  </div>
</template>

<script>

import Header from './components/Header.vue';
import MainTop from './components/Main_top.vue';
import MainBottom from './components/Main_bottom.vue';
import FooterTop from './components/Footer_top.vue';
import FooterBottom from './components/Footer_bottom.vue';

export default {
  name: 'App',
  components: {
   
    Header,
    MainTop,
    MainBottom,
    FooterTop,
    FooterBottom,

  }
}
</script>

<style lang="scss">

</style>
