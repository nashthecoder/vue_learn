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
import axios from 'axios'
export default {
  name: 'Dashboard',
  components: {
  
},
async created() {
  const { data } = axios.get("https://api.apify.com/v2/datasets/ZdYhQAMdc6OAGY1G0/items?format=json&clean=1");
  console.log(data);
}
}
</script>

<style>

</style>
