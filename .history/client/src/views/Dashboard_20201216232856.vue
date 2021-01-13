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
};

const options = {
  method: "GET",
  url: "https://covid-19-data.p.rapidapi.com/totals",
  headers: {
    "x-rapidapi-key": "8c3dc2e171msh41f5678235416dcp10242djsn97f569c61959",
    "x-rapidapi-host": "covid-19-data.p.rapidapi.com"
  }
};

axios.request(options).then(function (response) {console.log(response.data);
  })
    .catch(function (error) 
    {console.error(error);
  });
</script>

<style></style>
