<template>
  <div class="main-top">
    <div class="jumbotron">

    </div>
    <div class="container"> 
     <div class="current-series">
       <h2>current series</h2>
     </div> 
    

     <div class="cards">

       <div  v-for="(item,index) in cardList" :key=(index) class="card " >
         <img :src="item.thumb" alt="">
         <div class="series">{{item.series}}</div>
       </div>
      
       <div class="load-more">
         <h3>load more</h3>
       </div>

     </div>
    </div>
  </div>
  
</template>

<script>
export default {
  name:'Main-top',
  data(){
    return{
      cardList:[
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ]
    };
  },
 
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
  .main-top{
    background-color: #1C1C1C;
    .jumbotron{
      background-image: url('../assets/img/jumbotron.jpg');
      background-size: cover;
      height: 300px;
    };
    .container{
      position: relative;
      min-height: 100px;
      display: flex;
      align-items: center;
     .current-series{
       position: absolute;
       top: -30px;
       background-color: $azzurro;
       height: 40px;
       width: 250px; 
       margin-top: 10px ;
       cursor: pointer;
       h2{
         color: white;
         text-transform: uppercase;
         text-align: center;
         line-height: 40px;
       };
     } ;
     h1{
       color: wheat;
     };
     .cards{
       display: flex;
       flex-wrap: wrap;
       padding: 30px 0;
       justify-content: center;
       .card{
        height: calc(100vw / 8);
        width: calc(100vw / 8);
        
        img{
          object-fit: cover;
          object-position: 100% 0;
          width: 80%;
          height: 80%;
        };
        .series{
          text-transform: uppercase;
          color: white;
          margin-top: 10px;
          display: inline-block;
          font-size:8px;
          width: 80%;
        };
        
       };
       .load-more{
         background-color: $azzurro;
         height: 40px;
         width: 200px; 
         margin-top: 10px ;
         cursor: pointer;
         h3{
           color: white;
           text-transform: uppercase;
           text-align: center;
           line-height: 40px;
         };
       };
     };
    };
  };
 ;
</style>