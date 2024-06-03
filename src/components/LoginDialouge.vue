<template>
    <div>
      <v-form @submit.prevent="login">
        <v-text-field v-model="username" label="Username"></v-text-field>
        <v-text-field v-model="password" label="Password" type="password"></v-text-field>
        <v-btn type="submit" color="primary">Login</v-btn>
      </v-form>
    </div>
  </template>
  
  <script>
  export default {
    name: 'LoginComponent',
    data() {
      return {
        username: '',
        password: '',
      };
    },
    methods: {
      login() {
        console.log('Logging in...');
      },
    },
  };
  </script>
  