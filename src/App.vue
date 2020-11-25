<template>
<router-view>
  <Home/>
</router-view>
</template>

<script>
import Home from './components/Home'
export default {
  name: 'App',
  components: {
   Home,
  }
}
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Lato|Poppins|Roboto&display=swap");

* {
  margin:0px;
  padding: 0px;
  box-sizing:border-box;
  color:#000;
  font-family:"poppins",sans-serif;
}
</style>
