<script lang="ts">
  export default {
    data: () => ({ value: 0 }),
  }
</script>

<template>
    <v-layout class="overflow-visible" >
      <v-bottom-navigation
        v-model="value"
        active
        color="primary"
      >
        <v-btn>
          <v-icon>mdi-whatsapp</v-icon>
  
          WhatsApp
        </v-btn>
  
        <v-btn>
          <v-icon>mdi-instagram</v-icon>
  
          Instagram
        </v-btn>
  
        <v-btn>
          <v-icon>mdi-map-marker</v-icon>
  
          <span>Localização</span>
        </v-btn>
      </v-bottom-navigation>
    </v-layout>
  </template>