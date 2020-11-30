<template>
  <div class="container">
      <div class="container">
          <div class="texts">
            <p class="first-text">Best Quality Meals </p>
            <p class="second-text">NAmazing Variety <br>Of dishes <br>Starting Just GHS10</p>
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
.container {
  width: 100vw;
  background: #fff;
  height: 93vh;
  margin-left:38px

}
.texts{
    margin-top: 20px;
}

.first-text {
  font-size: 24px;
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
</style>