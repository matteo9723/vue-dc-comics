<template>
  <div class="main-bottom">
    <div class="container">
      <ul>
        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          digital comics
        </li>
        <li>
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          dc merchandise
        </li>
        <li>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          subscription
        </li>
        <li>
          <img src="..\assets\img\buy-comics-shop-locator.png" alt="">
          comic shop locator
        </li>
        <li>
          <img src="..\assets\img\buy-dc-power-visa.svg" alt="">
          dc power visa
        </li>
       
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name:'Main-bottom',
}
</script>

<style lang="scss" scoped>
  .main-bottom{
    height: 150px;
    background-color: #0282F9;
    .container{
      width: 80%;
      height: 100%;
      margin: 0 auto;
      display: flex;
      justify-content: space-around;
      align-content: center;
      ul{
        display: flex;
        list-style-type: none;
        justify-content: space-around;
        width: 100%;
        align-items: center;
        li{
          color: white;
          text-transform: uppercase;
          display: flex;
          align-items: center;
          img{
            height:  50px;
            margin: 0 10px;
          };
          &:last-child{
            img{
              width: 50px;
            }
          }
        }
      }
    }
  }
</style>