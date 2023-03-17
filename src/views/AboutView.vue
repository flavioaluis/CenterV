<script lang="ts">
import  FooterBar  from '../components/FooterBar.vue'

  export default {
    name: 'BrandView',
  components: {
    FooterBar,
  },
    data: () => ({
      items: [
        {
          title: 'Home',
          disabled: false,
          href: 'breadcrumbs_home',
        },
        {
          title: 'About',
          disabled: true,
          href: 'breadcrumbs_about',
        },
      ],
    }),
  }
</script>
<template>
  
   <v-row justify="space-between">
    <div>
    <v-breadcrumbs :items="items">
      <template v-slot:divider>
        <v-icon icon="mdi-chevron-right"></v-icon>
      </template>
    </v-breadcrumbs>
    </div>
      <v-col >
        <h1>About Us</h1>

          <p> 
          Lorem Ipsum is simply dummy text of the printing and typesetting 
          industry. Lorem Ipsum has been the industry's standard dummy text ever
          since the 1500s, when an unknown printer took a galley of type and 
          scrambled it to make a type specimen book. It has survived not only
          five centuries, but also the leap into electronic typesetting, 
          remaining essentially unchanged. It was popularised in the 1960s with
          the release of Letraset sheets containing Lorem Ipsum passages, and 
          more recently with desktop publishing software like Aldus PageMaker
          including versions of Lorem Ipsum.
          </p>

      </v-col>
      <v-col>
        <img alt="Foto Antiga" src="">
      </v-col>
  </v-row>
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
