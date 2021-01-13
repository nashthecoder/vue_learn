<template>
  <div class="sidebar">
    <div class="title">
      Simple Sidebar
    </div>
    <div class="menu-items">
      <router-link to="/dashboard">Dashboard</router-link>
      <router-link to="/line">Line</router-link>
      <router-link to="/bar">Bar</router-link>
      <router-link to="/doughnut">Doughnut</router-link>
      <router-link to="/pie">Pie</router-link>
      <router-link to="/radar">Radar</router-link>
      <router-link to="/polar-area">Polar Area</router-link>
      <router-link to="/bubble">Bubble</router-link>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.title {
  color: white;
  font-size: 24px;
  margin-top: 10px;
}
</style>
