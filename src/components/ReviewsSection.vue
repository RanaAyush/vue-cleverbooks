<template>
    <v-container class="customer-review">
      <v-row>
        <v-col cols="12" class="text-center">
          <h2>What Our Customers Say</h2>
        </v-col>
        <v-col cols="12" md="8" >
        <v-card class="review-card">
          <v-card-text>
            <p class="review-text">In today’s world of paid reviews, consumers prefer honest recommendations from real people. The Samosa Party is one such QSR brand that has gained immense recognition through its positioning on food delivery applications and word-of-mouth, becoming widely known by most households as their go-to snack preference.</p>
            <p class="review-text"> Throwing it back to 2015, Amit Nanwani, the founder of Samosa Party embarked on this journey with the sole intention of selling hygienic and authentic samosas, which came as a result of his constant battle between his eternal love for samosa and the struggle to find the ideal one that hit the right spots.</p>
            <p class="review-text"> <em>“From the beginning, the only goal was to detail and design samosas that were safe, hygienic, delicious, authentic, and free of all preservatives. All in one, to find a way to make the perfect samosas that involved least human intervention.”</em></p>
            <p class="review-author">~ Amit Nanwani, Founder</p>
          </v-card-text>
        </v-card>
        </v-col>
        <v-col cols="12" md="4">
        <v-card class="review-card image size">
            <!-- <v-img src="../assets/samosa.jpg" alt="not found" class="image"></v-img> -->
        </v-card>
      </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
  export default {
    name: 'ReviewsSection',
    data() {
      return {
        
      };
    },
  };
  </script>
  <style scoped>
    .image{
        background: url('../assets/samosa.jpg');
        background-size:cover;
        
    }
    .size{
        height: 475px;
        
    }
  .customer-review {
  padding: 40px 0;
}
  .review-card {
  border: 1px solid #ccc;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.review-text {
  font-size: 1.2rem;
  line-height: 1.6;
  margin: 20px 0;
}

.review-author {
  font-style: italic;
  margin-top: 10px;
}
  </style>