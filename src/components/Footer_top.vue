<template>
  <div class="footer-top"> 
    <div class="container">
      <div class="left">
        <div class="column">
          <ul>
            <li class="title"><h3>dc comics</h3></li>
            <li class="link"><a href="">Characters</a></li>
            <li class="link"><a href="">Comics</a></li>
            <li class="link"><a href="">Movies</a></li>
            <li class="link"><a href="">TV</a></li>
            <li class="link"><a href="">Games</a></li>
            <li class="link"><a href="">Videos</a></li>
            <li class="link"><a href="">News</a></li>
          </ul>
          <ul>
            <li class="title"><h3>shop</h3></li>
            <li class="link"><a href="">Shop DC</a></li>
            <li class="link"><a href="">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="column">
           <ul>
            <li class="title"><h3>dc</h3></li>
            <li class="link"><a href="">Terms Of Use</a></li>
            <li class="link"><a href="">Privacy policy(New)</a></li>
            <li class="link"><a href="">Ad Choices</a></li>
            <li class="link"><a href="">Advertising</a></li>
            <li class="link"><a href="">Jobs</a></li>
            <li class="link"><a href="">Subscriptions</a></li>
            <li class="link"><a href="">Talent Workshops</a></li>
            <li class="link"><a href="">CPSC Certificates</a></li>
            <li class="link"><a href="">Ratings</a></li>
            <li class="link"><a href="">Shop Help</a></li>
            <li class="link"><a href="">Contact Us</a></li>
          </ul>
        </div>
        <div class="column">
           <ul>
            <li class="title"><h3>sites</h3></li>
            <li class="link"><a href="">DC</a></li>
            <li class="link"><a href="">MAD Magazine</a></li>
            <li class="link"><a href="">DC Kids</a></li>
            <li class="link"><a href="">DC Universe</a></li>
            <li class="link"><a href="">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <div class="right">
        <img src="..\assets\img\dc-logo-bg.png" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:'Footer-top',
}
</script>

<style lang="scss" scoped>
.footer-top{
  height: 400px;
  background-image: url('../assets/img/footer-bg.jpg');
  .container{
    width: 80%;
    height: 100%;
    margin: 0 auto;
    display: flex;
    .left , .right{
      display: inline-block;
      width: 50%;
      height: 100%;
      display: flex;
    } ;
    .left{
      padding-top: 30px;
      .column{
        margin-right: 20px;
        ul{
          list-style-type: none;
          li{
            padding: 3px 0;
            a{
              color: gray;
              text-decoration: none;
            };
            h3{
              color: white;
              text-transform: uppercase;
              margin: 15px 0;
            }
          };
        };
      };
    };
    .right{
      align-items: center;
      img{
       width:  100%;
      };
    };
  };

};
</style>