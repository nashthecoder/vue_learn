<template>
  <div class="sidebar">
    <div class="title">
      Simple Sidebar
    </div>
    <div class="menu-items">
      <router-link 
        to="/dashboard"
        active-class="active"
        tag="button"
        exactclass="side-btn"
      >
        <div class="link-container">
          Dashboard
        </div>
      </router-link>
      <router-link
        to="/line"
        active-class="active"
        tag="button"
        exactclass="side-btn"
      >
        <div class="link-container">
          Line
        </div>
      </router-link>
      <router-link
        to="/bar"
        active-class="active"
        tag="button"
        exactclass="side-btn"
      >
        <div class="link-container">
          Bar
        </div>
      </router-link>
      <router-link 
        to="/doughnut"
        active-class="active"
        tag="button"
        exactclass="side-btn"
      >
        <div class="link-container">
          Doughnut
        </div>
      </router-link>
      <router-link to="/pie" active-class="active" tag="button" exact class="side-btn">
        <div class="link-container">
          Pie
        </div>
      </router-link>
      <router-link 
        to="/radar"
        active-class="active"
        tag="button"
        exactclass="side-btn"
      >
        <div class="link-container">
          Radar
        </div>
      </router-link>
      <router-link
        to="/polar-area"
        active-class="active"
        tag="button"
        exactclass="side-btn"
      >
        <div class="link-container">
          Polar Area
        </div>
      </router-link>
      <router-link
        to="/bubble"
        active-class="active"
        tag="button"
        exactclass="side-btn"
      >
        <div class="link-container">
          Bubble
        </div>
      </router-link>
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
.menu-items > * {
  margin-top: 60px;
}
.side-btn {
  border: none;
  padding: 16px 0px;
  cursor: pointer;
  font-size: 16px;
  font-weight: 500;
  color: white;
  background-color: transparent;
}
.side-btn:focus {
  outline: none;
}
.side-btn.active {
  position: relative;
  background-color: white;
  color: teal;
  font-weight: 600;
  margin-left: 10px;
  border-radius: 30px 0 0 30px;
}
.side-btn.active::before {
  top: -30px;
}
.side-btn.active::after {
  bottom: -30px;
}
.side-btn.active::before,
.side-btn.active::after {
  position: absolute;
  content: "";
  right: 0;
  height: 30px;
  width: 30px;
  background-color: white;
}
.side-btn.active .link-container::before {
  top: -60px;
}
.side-btn.active .link-container::after {
  bottom: -60px;
  z-index: 99;
}
.side-btn.active .link-container::before,
.side-btn.active .link-container::after {
  position: absolute;
  content: "";
  right: 0px;
  height: 60px;
  width: 60px;
  border-radius: 50%;
  background-color: #f6819d;
}
</style>
