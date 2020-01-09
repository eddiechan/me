<template>
  <div id="app" class="grid-container">
    <Sidemenu msg="The personal website of Eddie Chan. Under construction." class="sidemenu"/>
    <HelloWorld msg="Muji!" class="main"/>
  </div>
</template>

<script>
import Sidemenu from './components/Sidemenu.vue'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    Sidemenu, HelloWorld
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Acme');

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
}

.grid-container {
  display: grid;
  grid-template-areas:
    'sidemenu main';
  grid-gap: 0px;
  background-color: #FFF;
  padding: 0px;
}

.sidemenu {
  grid-area: sidemenu;
  background-color: teal;
  width: 200px;
}

.main {
  grid-area: main;
  text-align: left;
  background-color: pink;
}
</style>
