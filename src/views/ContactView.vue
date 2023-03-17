<script lang="ts">
import  FooterBar  from '../components/FooterBar.vue'

  export default {
    name: 'ContactView',
  components: {
    FooterBar,
  },
    data: () => ({
      items: [
        {
          title: 'Home',
          disabled: false,
          href: 'home',
        },
        {
          title: 'Contact',
          disabled: true,
          href: 'contact',
        },
      ],
    }),
  }
</script>

<template>
     <v-row justify="space-between">
    <div class="breadcrumbs">
    <v-breadcrumbs :items="items">
      <template v-slot:divider>
        <v-icon icon="mdi-chevron-right"></v-icon>
      </template>
    </v-breadcrumbs>
    </div>
      <v-col >
        <h1>Contact</h1>
        <v-divider class="border-opacity-25 w-50 pb-10"></v-divider>

        <v-card
              height="500"
              width="400"
              :class="['d-flex justify-start ', ]"
            >

            <div>
              <h3><v-icon>mdi-map-marker</v-icon>  Endereço</h3>
              <v-divider class="border-opacity-25 w-100" color="info"></v-divider>
              <p>Avenida Doutor Rômulo Cardillo, 453<br>
                Bairro João Pinheiro -
                Poços de Caldas, MG</p>
              
              <h3><v-icon>mdi-phone</v-icon>  Telefones</h3>
              <v-divider class="border-opacity-25 w-100" color="info"></v-divider>
              <p >Telefone Fixo: (35) 3722-2373<br>
                Celular: (35)99977-7688</p>

              <h3><v-icon>mdi-clock</v-icon>  Horário</h3>
              <v-divider class="border-opacity-25 w-100" color="info"></v-divider>
              <p class="phone">Segunda - Sexta: 8hs às 18hs <br>
              Não trabalhamos aos sábados e feriados.
                </p>
            </div>
            
        </v-card>

      </v-col>
      <v-col>
        <v-form></v-form>
      </v-col>
  </v-row>
    <FooterBar/> 
  </template>
  
  <style scoped>
.breadcrumbs {
  margin-left: 20px;

 }

div h1 {
  margin: 60px 0px 10px;
}
div h3 {
  text-align:center;
  margin: 25px 0px 10px;
}
div p {
  margin: 20px 30px;
  text-align: right;
 }
</style>