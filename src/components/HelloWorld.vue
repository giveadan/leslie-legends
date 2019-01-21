<template>
  <main>
    <div class="banner">
      <h1>Austin FC Leslie Legends</h1>
      <h3>The unofficial support group of Austin's MLS team</h3>
    </div>
      <img alt="Austin FC Supporters" src="/img/johns-1.jpg">
  </main>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
body {
  margin: 0;
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
</style>
