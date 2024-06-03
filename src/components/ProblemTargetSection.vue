<template>
    <v-container class="problem-target-section">
      <v-row>
        <v-col cols="12" class="text-center">
          <h2>Features of CleverBooks</h2>
        </v-col>
        <v-col cols="12" md="4" v-for="feature in features" :key="feature.title">
          <v-card>
            <v-img src="../assets/f.jpeg" alt="image not found" class="image"></v-img>
            <v-card-title>{{ feature.title }}</v-card-title>
            <v-card-text>{{ feature.description }}</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
  export default {
    name: 'ProblemTargetSection',
    data() {
      return {
        features: [
          { title: 'Feature 1', description: 'An easy-to-use interface that doesn’t require advanced training, support or documentation.' },
          { title: 'Feature 2', description: 'Automation for eliminating manual processes of business functions related to inventory management' },
          { title: 'Feature 3', description: 'Software integrations and automated features that minimize manual inventory updates or inputs.' },
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
  