<template>
  <v-app>
    <v-main>
      <HeroSection />
      <KeyProblemsSection />
      <KeyMetricsSection />
      <ReviewsSection />
      <ProblemTargetSection />
      <FooterSection />
    </v-main>
  </v-app>
</template>

<script>
import HeroSection from './components/HeroSection.vue';
import KeyProblemsSection from './components/KeyProblemsSection.vue';
import KeyMetricsSection from './components/KeyMetricsSection.vue';
import ReviewsSection from './components/ReviewsSection.vue';
import ProblemTargetSection from './components/ProblemTargetSection.vue';
import FooterSection from './components/FooterSection.vue';

export default {
  name: 'App',
  components: {
    HeroSection,
    KeyProblemsSection,
    KeyMetricsSection,
    ReviewsSection,
    ProblemTargetSection,
    FooterSection,
  },
};
</script>

<style>
body {
  font-family: 'Roboto', sans-serif;
}
</style>
