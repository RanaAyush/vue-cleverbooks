<template>
    <v-app-bar
      app
      color="secondary"
      dark
      class="hidden-navbar "
      
    >
      <v-toolbar-title>CleverBooks</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text>Home</v-btn>
      <v-btn text>Features</v-btn>
      <v-btn text>About</v-btn>
      <v-btn text>Contact</v-btn>
    </v-app-bar>
  </template>
  
  <script>
  export default {
    name: 'Navbar',
    data() {
      return {
        
      };
    },
    
  };
  </script>
  
  <style scoped>
  .hidden-navbar {
    opacity: 90%;
  }
  </style>
  