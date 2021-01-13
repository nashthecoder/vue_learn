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
  data() {
    return {
      arrDay: [],
      arrDayOfWeek: [],
      arrEquipment: [],
      arrExercise: [],
      arrExerciseInfo: [],
      arrExerciseCategory: []
    };
  },
  async created() {
    const { data } = await axios.get("https://covid-api.mmediagroup.fr/cases");
    console.log(data);
  }
};
</script>

<style></style>
