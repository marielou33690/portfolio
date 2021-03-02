<template>
  <div id="app">
    <Entete/>
    <section class="contenuPrincipal">
      <Accueil msg="Welcome to Your Vue.js App"/>
    </section>
    
    
  </div>
</template>

<script>
import Accueil from './components/Accueil.vue'
import Entete from './components/Entete.vue'

export default {
  name: 'App',
  components: {
    Accueil,
    Entete
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Bree+Serif&family=Pacifico&family=Roboto&family=Staatliches&display=swap');
html {
    box-sizing: border-box;
}

*, *::before, *::after{
    box-sizing: inherit;
}

body{
  margin: 0;
  background-color: #F6F6F6;
  font-family: 'Bree Serif', serif;
}
#app {
  color: white;
}
.contenuPrincipal{
   background-color: #FFA4B0;
}
</style>
