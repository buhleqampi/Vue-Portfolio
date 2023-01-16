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
  font-family: Georgia, 'Times New Roman', Times, serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height: 100px;

}

nav {
  padding: 30px;
  background-color: blue;

}

nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
  padding:5px;
  display: inline;
}

nav a.router-link-exact-active {
  color: orange;
}

body {
  background-color:#663399;
}
</style>
