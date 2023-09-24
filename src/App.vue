<script>
import Home from './Home.vue'
import About from './About.vue'
import NotFound from './Project.vue'

const routes = {
  '/': Home,
  '/about': About
}

export default {
  data() {
    return {
      currentPath: window.location.hash
    }
  },
  computed: {
    currentView() {
      return routes[this.currentPath.slice(1) || '/'] || NotFound
    }
  },
  mounted() {
    window.addEventListener('hashchange', () => {
		  this.currentPath = window.location.hash
		})
  }
}
</script>

<template>
  <nav>
   <div class="links">
    <ul>
      <li><a href="#/">Home</a></li> 
      <li><a href="#/project">project</a></li> 
      <li><a href="#/about">About</a></li> 
    </ul>
   </div> 
  </nav>
  <component :is="currentView" />
</template>
<style>
#app{
  margin-top: 2em;
}
nav{
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  
}
nav .links ul{
  display: flex;
  gap: 50px;
}

nav .links ul li{
  list-style: none;
}
nav .links ul li a{
  text-decoration: none;
  color: black;
}

</style>