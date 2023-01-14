<template>
  <nav>
    <router-link to="/">Home</router-link> 
    <router-link to="/about">About</router-link> 
    <router-link to="/projects">Projects</router-link> 
    <router-link to="/resume">Resume</router-link> 
    <router-link to="/testimonials">Testimonials</router-link> 
    <router-link to="/contact">Contact</router-link> 
    </nav>
    <router-view/>
    <body>

    </body>
    <Footer/>
</template>


<script>
import Footer  from './components/Footer.vue'
import nav from './components/NavBar.vue'
export default { 
  components: {nav, Footer } 
  }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height: 100px;

}

nav {
  padding: 30px;
  background-color:#ECECEC ;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
  padding:5px;
}

nav a.router-link-exact-active {
  color: #42b983;
}

body {
  background-color:#FF8B13;
}
</style>
