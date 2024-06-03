<template>
    <v-footer color="secondary" >
      <v-container>
        <CTASection />
        <v-row>
          <v-col class="text-center">
            <h4> CleverBooks is a supply chain software that provides companies tools for demand forecasting, inventory planning and more.</h4>
            <p>123 CleverBooks St, Booktown, BK 12345</p>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
  </template>
  
  <script>
  import CTASection from './CTASection.vue';
  export default {
    name: 'FooterSection',
    components:{
        CTASection,
    }
  };
  </script>
  <style scoped>
        v-footer {
        padding: 20px 0;
}
  </style>
  