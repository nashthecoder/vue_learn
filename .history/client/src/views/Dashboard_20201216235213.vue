<template>
  <div class="dashboard">
    <h1>Dashboard Example</h1>
    <v-container>
      <v-card-text></v-card-text>
      <v-card-text></v-card-text>
      <v-card-text></v-card-text>
    </v-container>
  </div>
</template>

<script>
import axios from "axios";

export default {
  components: {},
  async created() {
  const { data } = await axios.get("https://spoonacular-recipe-food-nutrition-v1.p.rapidapi.com/recipes/extract");
  }
};

</script>

<style></style>
