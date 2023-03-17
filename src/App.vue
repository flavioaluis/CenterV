<template>
    <v-container>
    <v-row justify="space-between">
      <v-col >
        <img alt="CV logo" src="./assets/logo1.png">  
      </v-col>
      <v-col :class="['pt-10']">        
            <v-card
              height="100"
              width="500"
              :class="['d-flex justify-center align-center ', ]"
            >
              <div> <h2>Endereço</h2>
              <p>Avenida Doutor Rômulo Cardillo, 434</p>
              <p>Bairro João Pinheiro, Poços de Caldas MG</p> </div>
            </v-card>
        </v-col>
      <v-col :class="['pt-10']">
            <v-card
              height="100"
              width="500"
              :class="['d-flex justify-center align-center ', ]"
            >
              <div><h2>Telefone</h2><p>(35)3722-2373</p><p>(35)99977-7688</p></div>
            </v-card>
        </v-col>
    </v-row>
  </v-container>
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
          <router-link to="/brands">Brands</router-link>
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

v-breadcrumbs {
  margin:30px;
}
</style>
