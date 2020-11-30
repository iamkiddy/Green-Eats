<template>
  <div class="main-nav-container">
    <div class="navbar">
      <div class="brand-content">
        <img src="../assets/green-eats-logo.jpg" width="120px" class="brand-logo">
      </div>
      <div class="nav-links">
        <div class="navlinks">
          <ul>
              <li>
                <router-link to="/" class="home-link">Home</router-link>
              </li>
              <li>
                <router-link to="/explore">Hot Deals</router-link>
              </li>
              <li>
                <router-link to="/hotdeal">Hot Deals</router-link>
              </li>
              <li>
                <router-link to="/categories">My Account</router-link>
              </li>
              <li>
                <img src="../assets/shopping-bag.svg" class="shopping-bag">
                <div class="bag-number">2</div>
              </li>
            </ul>
        </div>
        <div class="hide-me">
           <img src="../assets/shopping-bag.svg" class="shopping-bag bg-2">
           <img src="../assets/menu.svg" class="menu" width="24px">
           <div class="bag-number bn-2">2</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:"TopBarNavbar",
}
</script>

<style scoped>
*{
  margin:0px;
  padding:0px;
  box-sizing: border-box;
}
.navbar{
  display: flex;
}
.nav-links{
  margin-top:10px;
  margin-left: 580px;
}
.main-nav-container{
  padding:0 50px
}
.brand-name{
  margin-top:2rem;
}
.brand-logo{
  margin-top: -0.8rem;
}
ul {
  display: flex;
  flex-direction: row;
  margin-top: 30px;
}
.home-link {
  color: #7AC55E !important;
}
li {
  list-style: none;
  padding: 0 20px;
}
a {
  text-decoration: none;
  color: #333;
  font-weight: bold;
  transition: all 0.5s;
}
a:hover {
  color: #7AC55E;
}
.bag-number {
  position: relative;
  top: -50px;
  left:20px;
  background: #7AC55E;
  color: #ffffff;
  width: 1.25rem;
  border-radius: 50%;
  font-size: 0.75rem;
  font-weight: 500;
  text-align: center;
  line-height: 1.25rem;
}
.hide-me{
  display: none;
}

@media only screen and (max-width:600px){
  .main-nav-container{
    padding:0 0px;
  }
  .navlinks{
    display: none;
  }
  .hide-me{
    display: block;
    margin-left: -420px;
    margin-top: 25px;
  }
  .bg-2{
    padding:0 15px;
  }
  .bn-2{
    position: relative;
    left: 30px;
  }
.brand-logo{
  margin-left: -10px;
}
}
</style>