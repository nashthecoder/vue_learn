<template>
  <div class="dashboard">
    <h1>Dashboard Example</h1>
    <SideBarMenu />
    <v-container>
      <v-card-text></v-card-text>
      <v-card-text></v-card-text>
      <v-card-text></v-card-text>
    </v-container>
  </div>
</template>

<script>
import axios from "axios";
import SideBarMenu from '../components/SideBarMenu.vue';

export default {
  components:{
    SideBarMenu,
  },
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
    const { data } = await axios.get("https://api.covidtracking.com/v1/us");
    console.log(data);
  }
};
</script>

<style></style>
