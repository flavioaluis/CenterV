<template>
    <div class="d-block pa-6 bg--white">
      <img alt="CV logo" src="./assets/logo1.png">  
    </div>
    <div class="d-block pa-2 bg-red">
      <nav class="d-block pa-2 bg-red">
    <router-link to="/"><v-icon icon="mdi-home"></v-icon>Home </router-link> 
    <router-link to="/about">About</router-link> 
    <router-link to="/services">Services</router-link>
    <router-link to="/contact">Contact</router-link>
  </nav>
  <router-view/>
    </div>
</template>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav a {
 
  font-weight: bold;
  padding:40px;

}

nav a.router-link-exact-active {
  color: #42b983;
}

div img {

width:350px;
left:0;  
  
}
</style>
