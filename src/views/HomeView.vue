
<script lang="ts">
import { defineComponent } from 'vue';
import  FooterBar  from '../components/FooterBar.vue'
import CarrouselBar from '../components/CarrouselBar.vue'


export default defineComponent({
  name: 'HomeView',
  components: {
    FooterBar,
    CarrouselBar,
  },
});
</script>
<template>
  <CarrouselBar/>
  <FooterBar/>
</template>

<style>
 

</style>

