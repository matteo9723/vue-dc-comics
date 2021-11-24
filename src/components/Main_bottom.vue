<template>
  <div class="main-bottom">
    <div class="container">
      <ul>
        <li>ciao</li>
        <li>ciao</li>
        <li>ciao</li>
        <li>ciao</li>
        <li>ciao</li>
       
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
    background-color: teal;
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
      }
    }
  }
</style>