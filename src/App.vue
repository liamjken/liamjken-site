<template>
  <SiteHeader/>
  <router-view/>
</template>

<script>

import SiteHeader from './components/SiteHeader.vue'


export default {
  name: 'App',
  components: { SiteHeader }
}


</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}

body {
  margin: 0;
  background-image: url("./assets/backdrop.jpg") ;
}
</style>
