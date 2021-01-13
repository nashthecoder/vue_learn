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
    const { data } = await axios.get("https://wger.de/api/v2/");
    console.log(data);
  }
};
</script>

<style></style>
