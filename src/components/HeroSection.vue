<template>
    <v-container fluid class="hero-section">
        <Navbar/>
        <div class="text-center rattach">
          <h1>CleverBooks</h1>
          <p>Innovating the Future of Inventory Management</p>
          
          <v-btn color="primary" large @click="showLoginDialog">Get Started</v-btn>
          <v-dialog v-model="loginDialog" max-width="500px">
            <v-card>
                <v-card-title>Login</v-card-title>
                <v-card-text>
                <LoginDailouge />
                </v-card-text>
                <v-card-actions>
                <v-btn color="primary" @click="loginDialog = false">Close</v-btn>
                </v-card-actions>
            </v-card>
        </v-dialog>
        </div>
    </v-container>
  </template>
  
  <script>
    import Navbar from './Navbar.vue'
    import LoginDailouge from './LoginDialouge.vue'
  export default {
    name: 'HeroSection',
    components:{
        Navbar,
        LoginDailouge,
    },
    data() {
    return {
      loginDialog: false,
    };
  },
  methods: {
    showLoginDialog() {
      this.loginDialog = true;
    },
  },
  };
  </script>
  
  <style scoped>
    
    .rattach{
        position: absolute;
        left: 80px;
        top: 230px;

    }
  .hero-section {
    background-image: url('../assets/hero-img.jpg');
    background-size: cover;
    color: white;
    padding: 100px 0;
    height: 80vh;
  }
  </style>
  