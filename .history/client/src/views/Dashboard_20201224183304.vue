<template>
  <SideBarMenu />
</template>

<script>
import axios from "axios";
import SideBarMenu from '../components/SideBarMenu.vue';

export default {
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
