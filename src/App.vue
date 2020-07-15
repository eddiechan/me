<template>
  <div class="wrapper">
    <div class="top-bar"></div>
    <div class="title">Eddie Chan</div>
    <div class="about">
      <p>Hello 👋🏻 I'm a software developer in Vancouver 🇨🇦</p>
      <p>I like to drink coffee, take photos, <a href="https://www.strava.com/athletes/18698106" target="_blank">run</a>, cook for my kids, and attempt to stay up-to-date with the latest in the tech world (partly what this little site is for).</p>
    </div>
    <div class="content">
      <div class="links">Obligatory Links</div>
      <div class="resume">Resume</div>
    </div>
  </div> 
</template>

<script>
// import Sidemenu from './components/Sidemenu.vue'
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    // Sidemenu, HelloWorld
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Love+Ya+Like+A+Sister&display=swap');
@import url('https://fonts.googleapis.com/css?family=Muli&display=swap');

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
}

.wrapper {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 0px;
  grid-auto-rows: min-content;
  margin: 1px;
}

.top-bar {
  grid-column: 1 / 4;
  grid-row: 1 / 2;
  height: 10px;
  background-color: rgb(43, 110, 186);
}

.title {
  font-family: 'Love Ya Like A Sister', cursive;
  font-size: 60px;
  grid-column: 1 / 4;
  grid-row: 2 / 3;
  padding: 10px;
  background-color: white;
}

.about {
  grid-column: 1 / 4;
  grid-row: 3 / 4;
  padding: 0px 10px 10px 10px;
  color: rgb(56, 56, 56);
  background-color: white;
  font-family: 'Muli', sans-serif;
  max-width: 600px;
}

.content {
  grid-column: 1 / 4;
  grid-row: 4 / 5;

  font-family: 'Muli', sans-serif;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 10px;
  grid-auto-rows: min-content;
  
  padding: 10px;
  margin: 1px;
}

.links {
  grid-column: 1 / 2;
  grid-row: 1 / 2;
  background-color: blue;
}

.resume {
  grid-column: 2 / 4;
  grid-row: 1 / 2;
  background-color: pink;
}




body {
    margin: 0;
}

a:link {
  text-decoration: underline;
  color: rgb(56, 56, 56);
}

a:visited {
  text-decoration: none;
  color: rgb(56, 56, 56);
}

a:hover {
  text-decoration: underline;
  color: rgb(255, 80, 0);
}

a:active {
  text-decoration: underline;
}
</style>
