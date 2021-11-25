<template>
  <div class="container">
    <div class="left">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div class="right">
      <ul>
        <a href="" >
          <li>characters</li>
          <div class="underline "></div>
        </a>
        <a href=""><li>comics</li></a>
        <a href=""><li>movies</li></a>
        <a href=""><li>tv</li></a>
        <a href=""><li>games</li></a>
        <a href=""><li>collectibles</li></a>
        <a href=""><li>videos</li></a>
        <a href=""><li>fans</li></a>
        <a href=""><li>news</li></a>
        <a href=""><li>shop</li></a>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name:'Header',
}
</script>

<style lang="scss" scoped>
@import "../assets/img/style/vars.scss";
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
        li{
          margin: 0 10px;
          text-transform: uppercase;
        };
        .underline{
          width: 80px;
          height: 5px;
          background-color: $azzurro;
          position: absolute;
          bottom: 0;
          left: 50%;
          transform: translateX(-50%);
        }
      };
    };
  };

</style>