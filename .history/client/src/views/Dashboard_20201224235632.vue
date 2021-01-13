<template>
  <div id="sidebar">
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
  </div>
</template>

<script>
export default {
  name: "dashboard",
  components: {},
  data() {
    return {};
  }
};
</script>

<style scoped>
#sidebar {
  display: flex;
  align-content: left;
}
</style>
