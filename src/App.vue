<template>
  <div id="app">
    <router-link to="/CreateStore"></router-link>
    <router-link to="/"></router-link>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;1,100&display=swap');
html {
  box-sizing: border-box;
  font-size: 16px;
}

*, *:before, *:after {
  box-sizing: inherit;
}

body, h1, h2, h3, h4, h5, h6, p, ol, ul {
  margin: 0;
  padding: 0;
  font-weight: normal;
}

ol, ul {
  list-style: none;
}

img {
  max-width: 100%;
  height: auto;
}
#app {
  font-family: 'Poppins', sans-serif;
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
button:hover{
        box-shadow: 0 0px 2.2px #665eff1f,
            0 0px 5.3px #665eff0a,
            0 0px 10px #665eff0a,
            0 0px 17.9px #665eff0a,
            0 0px 33.4px #665eff0a,
            0 0px 80px #665eff0a
    }

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
