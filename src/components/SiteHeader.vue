<template>
    <div>
        <div><img alt="logo" src="../assets/logo.svg" class="logo"></div>
        <nav>
    <router-link to="/">Home</router-link> 
    <router-link to="/about">About</router-link>
  </nav>

    </div>
</template>

<script>

</script>

<style>
nav {
  padding: 10px 30px;
}

nav a {
  font-weight: bold;
    color: white;
    text-decoration: none;
    background: #404040;
    border: solid 2px #404040;
    padding: 5px 10px;
    display: inline-block;
    transform: skew(-13deg, 0deg);
    box-shadow: rgba(9, 30, 66, 0.25) 0px 4px 8px -2px, rgba(9, 30, 66, 0.08) 0px 0px 0px 1px;
    margin: 0px 5px;
}

nav a.router-link-exact-active {
  color: #fe2300;
    background: rgb(241 236 236);
    border: solid 2px #fe2300;
}

img.logo{
  width: 300px;
}
</style>