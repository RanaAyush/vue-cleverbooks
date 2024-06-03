<template>
    
    <v-container class="key-problems-section">
      <v-row>
        <v-col cols="12" class="text-center">
          <h2>Key Problems Solved by CleverBooks</h2>
        </v-col>
        <v-col cols="12" md="4" v-for="problem in problems" :key="problem.title">
          <v-card>
            <v-img src="../assets/1.png" alt="Image not found" class="image"></v-img>
            <v-card-title>{{ problem.title }}</v-card-title>
            <v-card-text>{{ problem.description }}</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
  export default {
    name: 'KeyProblemsSection',
    data() {
      return {
        problems: [
          { title: 'What to order', description: 'Get accurate demand and days to stock out. Automate purchase planning so you can always have what you need for your next sales cycle.' },
          { title: 'When to order', description: 'Have up-to-date inventory, storage, sales velocity, and demand. Get timely order suggestions so you are never left guessing.' },
          { title: 'How much to stock', description: 'Get inventory requirements for every node, for every SKU. So you avoid out-of-stock situations, even during demand spikes.' },
        ],
      };
    },
  };
  </script>
  <style scoped>
    .image{
        height: 200px;
    }
  </style>
  