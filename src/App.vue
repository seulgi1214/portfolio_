<template>
  <div>

  </div>
  <!-- <div id="nav">
    <router-link to="/">Home</router-link> 
    <router-link to="/about">About</router-link> 
  </div> -->
  <router-view/>
</template>


<style>


body {
  background: url("assets/img/bg.png");
}

#app {
  font-family: 'Noto Sans KR', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  max-width: 1000px;
  color: #333333;
  margin: 0 auto;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

body, html, h1, h2, h3, h4, h5, p {
  margin: 0;
  padding: 0;
}

ul, ol {
  list-style: none;
  margin: 0;
  padding: 0;
} 


</style>
