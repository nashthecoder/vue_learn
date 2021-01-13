<template>
  <div id="sidebar" md="6">
    <ul>
      <li><a href="/line">Line</a></li>
      <li><a href="/bar">Bar</a></li>
      <li><a href="/doughnut">Doughnut</a></li>
      <li><a href="/pie">Pie</a></li>
      <li><a href="/radar">Radar</a></li>
      <li><a href="/polar-area">Polar Area</a></li>
      <li><a href="/bubble">Bubble</a></li>
      <li><a href="/scatter">Scatter</a></li>
    </ul>
    <div id="sidebar-btn" v-on:click="exibir()">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </div>
</template>

<script>
import $ from "jquery";
export default {
  name: "dashboard",
  props: ["mostrar"],
  methods: {
    exibir: () => {
      $("#sidebar").toggleClass("visible");
    }
  }
};
</script>

<style scoped>
#sidebar {
  display: flex;
}
</style>
