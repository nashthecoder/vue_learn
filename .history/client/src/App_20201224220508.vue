<template>
  <div id="app">
    <ResponsiveNav 
    :nav-links="navLinks"

		background="#fff"
		link-color="#777"
		hoverBackground="#ddd"
    />
    <router-view />
        </div>
</template>
<script>
import ResponsiveNav from "@/components/ResponsiveNav"
export default {
  components: {
    ResponsiveNav
  },
  data: () => ({
    navLinks: [
      {
        text: 'Contact',
		path: '/contact',
		icon: 'ion-ios-megaphone'
      },
      {
        text: 'About',
		path: '/about',
		icon: 'ion-ios-business'
      },
      {
        text: 'Blog',
		path: '/blog',
		icon: 'ion-ios-bonfire'
      },
      {
        text: 'Portfolio',
		path: '/portfolio',
		icon: 'ion-ios-briefcase'
      }
    ]
  })
}
</script>
<style>
body {
  margin: 0;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
