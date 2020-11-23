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
* {
  margin:0px;
  padding: 0px;
  box-sizing:border-box;
  color:#000
}
</style>
