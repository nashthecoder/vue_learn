<template>
  <SideBarMenu />
</template>

<script>
import axios from "axios";
import SideBarMenu from '../components/SideBarMenu.vue';

export default {
  components: {
    SideBarMenu
  },
  data() {
    return {};
  },
  async created() {
    const { data } = await axios.get("https://api.covidtracking.com/v1/us");
    console.log(data);
  }
};
</script>

<style></style>
