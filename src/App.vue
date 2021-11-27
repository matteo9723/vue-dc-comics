<template>
  <div id="app">
    <Header :menu="Data"/>
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
import Data from './assets/data/data.js';

export default {
  name: 'App',
  data(){
    return{

      Data
     
    }
  },
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
  @import "./assets/style/vars.scss";
  
  // @import url('https://fonts.googleapis.com/css2?family=Lato&family=Open+Sans:ital@1&family=Roboto&display=swap');

  @import "./assets/style/font.scss";
  *{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
</style>
