<template>
  <div id="itemssection">
    <div class="items">
      <div class="card c1">
        <h1 class="card-header">Phones</h1>
        <p class="card-para">Apple</p>
        <img src="../assets/eat-the-rainbow.png" class="food-img" />
      </div>
      <div class="card c1">
        <h1 class="card-header">Men</h1>
        <p class="card-para">Nike 2020</p>
        <img src="../assets/eat-the-rainbow.png" class="food-img" />
      </div>
      <div class="card c1">
        <h1 class="card-header">Laptop</h1>
        <p class="card-para">Apple</p>
        <img src="../assets/eat-the-rainbow.png" class="food-img" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "itemssection",
};
</script>

<style scoped>
.itemssection {
  width: 100vw;
  color: #fff;
  margin-left: 20px;
  height: 100vh;
  background:#E9E8E4 !important;
}

.items {
  margin-left: 100px;
  margin-top: 100px;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
}
.card {
  border: 1px solid lightgray;
  width: 350px;
  height: 270px;
  transition: all 0.5s;
}
.card:hover {
  background: #64DB61;
  opacity: 0.8;
  color: rgb(158, 150, 150);
}
.card-header {
  font-family: "poppins", sans-serif;
  font-weight: bold;
  font-size: 28px;
  margin-top: 30px;
  margin-left: 30px;
  color: #000;
}
.card-para {
  font-family: "poppins", sans-serif;
  margin-left: 30px;
  position: relative;
  top: 20px;
}
.card-img {
  width: 120px;
  position: relative;
  top: -80px;
  margin-left: 200px;
}
.nike {
  width: 300px;
  margin-left: 50px;
}
.laptop {
  width: 300px;
  margin-left: 90px;
  top: 5px;
}
.food-img{
    width:300px;
    position: relative;
    top:-70px;
    left:70px
}
@media only screen and (max-width: 600px) {
    .items{
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 30px;
        margin-left:15px;

    }
}
</style>