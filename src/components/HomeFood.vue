<template>
  <div class="main">
      <div class="container">
          <div class="texts">
            <p class="first-text">Best Quality Meals </p>
            <p class="second-text">Namazing Variety <br>Of dishes <br>Starting Just GHS10</p>
            <button class="sec-btn">SHOP NOW</button>
          </div>
          <div class="img-content"></div>
      </div>
  </div>
</template>

<script>
export default {
    name:"HomeFood"
}
</script>

<style scoped>
.main{
   background: #EAE9E7;
   margin-top:-20px;    
}
.container {
  width: 100vw;
  background: #EAE9E7;
  height: 85vh;
  margin-left:38px

}
.texts{
 position: relative;
 top:50px;
 left: 40px;
}
.first-text {
  font-size: 16px;
}
.second-text {
  font-family: "Liu Jian Mao Cao", cursive;
  font-size: 60px;
  margin-top: 20px;
}
.sec-btn {
  min-width: 161px;
  height: 46px;
  margin-top: 50px;
  border-radius: 23px;
  background: #7AC55E;
  border: none;
  font-weight: bold;
  color: #fff;
  font-size: 15px;
  transition: all 0.5s;
  cursor: pointer;
  font-family: "poppins", sans-serif;
}
.sec-btn:hover {
  background: #333;
}
@media only screen and (max-width:600px){
    .container{
        width: 100vw;
        height: 84.5vh;
    }
    .texts{
        position: releative;
        left: -20px;
        top: 100px;
    }
    .second-text{
        font-size: 30px;
    }
}
</style>