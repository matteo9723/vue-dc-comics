<template>
  <div class="container">
    <div class="left">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div class="right">
      <ul>
        
          <li @click="item.current='true'" v-for="(item , index) in menu" :key="index">
            <a :class="{active: item.current}" href="#">{{item.text}}</a>
            <div class="underline " :class="{block: item.current}"></div>
          </li>
        
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name:'Header',
  props:{
    menu: Array
  },
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
 

  .container{
    width: 80%;
    height: 120px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .right{
   
    height: 100%;
   
    ul{
      height: 100%;
      display: flex;
      list-style-type: none;
      li{
        margin: 0 10px;
        text-transform: uppercase;
        position: relative;
       .active{
         color: $azzurro;
       } ;
       a{
        position: relative;
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        color: rgb(73, 72, 72);
        text-decoration: none;
        font-weight: bolder;
        &:hover{
          color: $azzurro;
        };
       }; 
       .underline{
         width: 80%;
        height: 5px;
        background-color: $azzurro;
        position: absolute;
         bottom: 0;
        left: 50%;
        transform: translateX(-50%);
        display: none;
       }
       .block{
        display: block;
       } 
      };
    };
  };

</style>