<template>
  <div id="app">
    <Header :menu="linksList"/>
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
  data(){
    return{
      linksList:[
        {
          text: 'characters',
          current: true
        },
        {
          text: 'comics',
          current: false
        },
        {
          text: 'movies',
          current: false
        },
        {
          text: 'tv',
          current: false
        },
        {
          text: 'games',
          current: false
        },
        {
          text: 'collectibles',
          current: false
        },
        {
          text: 'videos',
          current: false
        },
        {
          text: 'fan',
          current: false
        },
        {
          text: 'news',
          current: false
        },
        {
          text: 'shop',
          current: false
        },
      ]
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
  @import url('https://fonts.googleapis.com/css2?family=Lato&family=Open+Sans:ital@1&family=Roboto&display=swap');
  *{
    font-family: 'Roboto';
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
</style>
