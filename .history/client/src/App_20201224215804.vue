<template>
  <div id="app">
    <ResponsiveNav 
    :nav-links="navLinks"
		:image-path="require('./assets/logo.png')"
		background="#fff"
		link-color="#777"
		hoverBackground="#ddd"
    />
          <router-view />
        </div>
      </div>
    </div>
  </div>
</template>
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
