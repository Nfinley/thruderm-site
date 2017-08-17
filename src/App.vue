<template>
  <div id="app">
    <div class="nav-container">
      <ul>
        <li><img src="./assets/thruderm.png" class="logo-icon"></li>
        <li><a href="#home" target="_blank">Home</a></li>
        <li><a href="#store" target="_blank">Store</a></li>
        <li><a href="#contact" target="_blank">Contact</a></li>
      </ul>
    </div>


    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app',
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #0a2239;
  margin-top: 60px;
}
ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
  color: #474D4E;
}
a {
  color: #474D4E;
}
.logo-icon {
  height: 100px;
}
</style>
