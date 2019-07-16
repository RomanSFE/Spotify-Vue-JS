<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/spot">Spot</router-link>
    </div> -->
    <Menu/>
    <router-view/>
  </div>
</template>

<script>
import Menu from '@/components/Menu.vue'
export default {
  components: {
    Menu
  }
}
</script>


<style lang="scss">
@import url("https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css");
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body{
	background-color: #3c434c;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #fff;
    padding: 5px 10px 10px 10px;
    font-size: 15px;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
