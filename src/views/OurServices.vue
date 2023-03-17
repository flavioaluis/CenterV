<script lang="ts">
import  FooterBar  from '../components/FooterBar.vue'

  export default {
    name: 'OurServices',
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
          title: 'Services',
          disabled: true,
          href: 'services',
        },
      ],
    }),
  }
</script>

<template>
    <div>
    <v-breadcrumbs :items="items">
      <template v-slot:divider>
        <v-icon icon="mdi-chevron-right"></v-icon>
      </template>
    </v-breadcrumbs>
    </div>
    <h1>Services</h1>

    <FooterBar/> 
  </template>
  
  <style scoped>
div  {
  margin-left: 30px;

 }

div h1 {
  margin: 60px 60px 30px;
}
 div p {
  margin: 30px 60px 30px;
 }

 
</style>