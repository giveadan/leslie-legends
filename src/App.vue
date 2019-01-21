<template>
  <div id="app">
    <div class="hero">
      <img alt="Austin Leslie" src="./assets/leslie.png">
    </div>
    <div class="banner">
      <h1>Austin FC <span class="text-nowrap">Leslie Legends</span></h1>
      <h3>The unofficial support group of Austin's MLS team</h3>
    </div>
    <div class="flexing">

      <div class="flex-content">
        <blockquote>
          &ldquo;Damn. I missed all the good swag. They are out of scarves and hats now.&rdquo; 
        </blockquote>
        <blockquote>
          &ldquo;Just being here is getting me jacked up I'm ready to crush dozens of lone stars at these games&rdquo; 
        </blockquote>
        <p>John's reaction to attending the official announcement ceremony</a></p>
      </div>
      <div class="flex-img">
        <img alt="Austin FC Supporters" src="./assets/johns-1.jpg" />
      </div>
    </div>
    <div class="flexing">
      <div class="flex-img">
        <img alt="Austin FC Supporters" src="./assets/johns-2.jpg" />
      </div>
      <div class="flex-content">
        <blockquote>
          &ldquo;Awful... Do they realize one of our own would have to mean its a player from Austin who came up through the youth system that is like 7 years away from producing a person who would fit that mold? Just... So bad&rdquo; 
        </blockquote>
        <p>Other John's thoughts about <a href="https://twitter.com/AlyssaMGoard/status/1085294423204941825" target="_blank">the official Austin FC chant hymnal</a></p>
      </div>
      
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style lang="scss">
blockquote {
  font-size: 2.2em;
  font-family: serif;
  font-style: italic;
  font-weight: lighter;
  text-align: left;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  margin: 0;
}
.hero {
  display: flex;
  justify-content: center;
  align-items: flex-end;
}
.text-nowrap {
  white-space: nowrap;
}
.flexing {
  display: flex;
  align-items: center;
}
.flex-content {
  flex: 3;
}
.flex-img {
  flex: 2;
  img {
    width: 100%;
  }
}
h1 {
  margin: 0;
}
h3 {
  margin: 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.banner {
  background: green;
  color: white;
  padding: 10px;
}

@media screen and (max-width:900px) {
  blockquote {
    font-size: 1.5em;
  }
}

@media screen and (max-width:500px) {
  .flexing {
    flex-direction: column;
  }
  .flexing + .flexing {
    flex-direction: column-reverse;
  } 
  .hero img {
    width: 40%;
  }
}

</style>
