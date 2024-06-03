<template>
    <v-container class="cta-section" text-center>
    <h2>Grow Faster Than You Think</h2>
    <p>Join CleverBooks today and revolutionize your inventory management.</p>
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
  </v-container>
  </template>
  
  <script>
  import LoginDailouge from './LoginDialouge.vue'
  export default {
    name: 'CTASection',
    components:{
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
.cta-section {
  margin: 20px 0;
  padding: 20px;
  text-align: center;
}
</style>