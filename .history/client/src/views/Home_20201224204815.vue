<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/chartjs.png" />
    <Home msg="Data Visualization" />
  </div>
</template>

<script>
// @ is an alias to /src
import Home from "@/components/Home.vue";

export default {
  name: "home",
  components: {
    Home,
  }
};
</script>
