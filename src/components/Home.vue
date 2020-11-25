<template>
  <div class="home">
    <TopBarNavbar />
    <HomeFood />
  </div>
</template>

<script>
import TopBarNavbar from './TopBarNavbar'
import HomeFood from './HomeFood'
export default {
  name: 'Home',
  components:{
    TopBarNavbar,
    HomeFood
  }

}
</script>


<style scoped>

</style>
