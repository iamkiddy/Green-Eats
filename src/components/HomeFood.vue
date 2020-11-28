<template>
  <div class="navcarousel">
    <div class="container">
      <div class="container-1">
        <header>
          <h1 class="brand-name">
            <router-link to="/"><img src="../assets/green-eats-logo.jpg" class="brand-pic" width="54px"></router-link>
          </h1>
          <nav>
            <ul>
              <li>
                <router-link to="/" class="home-link">Home</router-link>
              </li>
              <li>
                <router-link to="/explore">Explore</router-link>
              </li>
              <li>
                <router-link to="/hotdeal">Hot Meals</router-link>
              </li>
              <li>
                <router-link to="/categories">Categories</router-link>
              </li>
              <li>
                <router-link to="/shops">Shops</router-link>
              </li>
            </ul>
          </nav>
          <div class="shop-icons">
            <img src="../assets/search.svg" class="search" />
            <img src="../assets/shopping-bag.svg" class="bag" />
            <img src="../assets/user.svg" class="user" width="25px"/>
          </div>
          <div class="bag-number">2</div>
        </header>
        <section class="sec1">
          <div class="texts">
            <p class="second-text">Today's Meal</p>
            <button class="sec-btn">ORDER NOW</button>
          </div>
          <div class="image">
          </div>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "navcarousel",
  components: {
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Liu+Jian+Mao+Cao&display=swap");


.container {
  background-image: url("../assets/bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  height: 93vh;
  margin: 0px !important;

}

.container-1 {
  font-family: "poppins", sans-serif;
  margin-left: 100px;
  margin-right: 100px;
}

header {
  display: flex;
  flex-direction: row;
}
.brand-name {
  margin-top: 18px;
}
ul {
  display: flex;
  flex-direction: row;
  margin-top: 30px;
}
.home-link {
  color: #64DB61 !important;
}
li {
  list-style: none;
  padding: 0 20px;
}
a {
  text-decoration: none;
  color: #fff;
  font-weight: bold;
  transition: all 0.5s;
}
a:hover {
  color: #64DB61;
}
.shop-icons {
  margin-top: 30px;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 30px;
  position: relative;
  right: -402px;
}
img {
  cursor: pointer;
  transition: all 0.5s;
}
img:hover {
  color: #64DB61;
}
.bag-number {
  position: absolute;
  right: 190px;
  top: 55px;
  background: #64DB61;
  color: #ffffff;
  width: 1.25rem;
  border-radius: 50%;
  font-size: 0.75rem;
  font-weight: 500;
  text-align: center;
  line-height: 1.25rem;
}
.texts {
  margin-top: 130px;
}
.first-text {
  font-size: 28px;
}
.second-text {
  font-family: "Liu Jian Mao Cao", cursive;
  font-size: 60px;
  margin-top: 20px;
}
.sec-btn {
  width: 161px;
  height: 46px;
  margin-top: 50px;
  border-radius: 23px;
  background: #64DB61;
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
.img-main {
  position: absolute;
  top: 150px;
  right: 200px;
  width: 500px;
  height: 450px;
  object-fit: contain;
  border: none;
}
@media only screen and (max-width: 600px) {
  nav {
    display: none;

  }
  .container{
    height: 100vh;
    width:100vw;
  }
  .shop-icons{
    margin-left: -260px;
  }
  .bag-number{
    position: absolute;
    left:300px;
    top:10px;
  }
  .search{
    width: 20px;
  }
  .bag{
    width:20px;
  }
  .user{
    width: 20px;
  }
  .img-main{
    width:250px;
    margin-top: -100px;
    margin-right: -180px;
    display: none;
  }
  .second-text{
    font-size: 30px;
    margin-left: -90px;
  }
  .sec-btn{
    width: 150px;
    height: 40px;
    margin-left:-90px;
    font-size:16px
  }
  .texts{
    z-index: 1;
  }
  .brand-pic{
    margin-left: -90px;
  }
  .texts{
    position: relative;
    top:100px;
    left:200px;
  }
  .second-text{
    color:#fff
  }
}
</style>
