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
  name: "Dashboard",
  components: {},
  async created() {
    const { data } = axios.get("https://covid-19-data.p.rapidapi.com/totals");
    console.log(data);
  }
};
</script>

<style></style>
