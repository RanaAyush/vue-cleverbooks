<template>
    <v-container class="key-metrics-section">
      <v-row>
        <v-col cols="12" class="text-center">
          <h2>Why Choose CleverBooks?</h2>
        </v-col>
        <v-col cols="12" md="4" v-for="metric in metrics" :key="metric.title">
          <v-card>
            <v-img  class="image" src="../assets/3.png" alt="image not found"></v-img>
            <v-card-text>{{ metric.description }}</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
  export default {
    name: 'KeyMetricsSection',
    data() {
      return {
        metrics: [
          { description: 'how much stock to order at what time.' },
          { description: 'Satisfies customers with timely deliveries.' },
          { description: 'Prevent overspending on warehouse storage.' },
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
  