<template>
  <div class="footer-bottom">
    <div class="container">
      <div class="box">
        <div class="btn">sign-up now!</div>
        <div class="social">
          <h3>follow us</h3>
          <img src="..\assets\img\footer-facebook.png" alt="">
          <img src="..\assets\img\footer-periscope.png" alt="">
          <img src="..\assets\img\footer-pinterest.png" alt="">
          <img src="..\assets\img\footer-twitter.png" alt="">
          <img src="..\assets\img\footer-youtube.png" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:'Footer-bottom',
}
</script>

<style lang="scss" scoped>
@import "../assets/img/style/vars.scss";
  .footer-bottom{
    background-color: rgb(73, 71, 71);
    height: 120px;
    .container{
      width: 80%;
      height: 100%;
      margin: 0 auto;
      .box{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        .btn{
          padding: 10px;
          color: white;
          text-transform: uppercase;
          border: 3px solid $azzurro;
          cursor: pointer;
        };
        .social{
          display: flex;
          align-items: center;
          h3{
            text-transform: uppercase;
            color: $azzurro;
            margin: 0 30px,
          };
          img{
              margin: 0 10px;
              cursor: pointer;
          };
        };
      };
    };
  };
</style>