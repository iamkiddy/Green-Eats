<template>
  <div class="home">
    <TopBarNavbar />
    <HomeFood />
    <Category />
  </div>
</template>

<script>
import TopBarNavbar from './TopBarNavbar'
import HomeFood from './HomeFood';
import Category from './Category';
export default {
  name: 'Home',
  components:{
    TopBarNavbar,
    HomeFood,
    Category
  }

}
</script>


<style>
.home{
  overflow: hidden;
}
</style>
