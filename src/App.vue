<template>
    <div class="h-25 w-0 bg--white">
      <img alt="CV logo" src="./assets/logo1.png">  
    </div>
    <div>
      <v-divider
      class="ms-4"
      inset
      vertical
    ></v-divider>
      <nav class=" bg-red">
        
        <v-toolbar-items>
        
          <router-link to="/">Home </router-link> 
            <v-divider vertical></v-divider>
          <router-link to="/about">About</router-link> 
            <v-divider vertical></v-divider>
          <router-link to="/services">Services</router-link>
            <v-divider vertical></v-divider>
          <router-link to="/contact">Brands</router-link>
          <v-divider vertical></v-divider>
          <router-link to="/contact">Contact</router-link>
          
        </v-toolbar-items>
  </nav>
  <router-view/>
    </div>
</template>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  color: #2c3e50;
}

nav a {
 
  font-weight: bold;
  width:100%;
  padding: 15px;
  text-align: center;

}

nav a.router-link-exact-active {
  color: #42b983;
}

div img {
  padding-top: 30px;
  width:300px;  
}
</style>
