<template>
  <Nav/>
  <router-view/>
  <Footer/>

</template>


<script>

import Nav from './views/Nav.vue'
import Footer from './views/Footer.vue'
export default {
  components :{
    Nav,
    Footer
  }
}
</script>


<style>


body {
  background: url("assets/img/bg.png");
}

#app {
  font-family: 'Noto Sans KR', Helvetica, Arial, sans-serif;
  max-width: 1000px;
  color: #333333;
  margin: 0 auto;
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

a {
  color: #333333;
  text-decoration: none;
}

  .common_container {
    background: #ffffff;
    border-radius: 5px; 
    padding: 30px;
  }

.common_title {
    text-align: left; 
    position: relative; 
    padding-left: 15px;
  }

  .common_title::before {
    background-color: #BD97CB;  
    content: ""; 
    position: absolute;
    top: 50%;  
    left: 0;  
    width: 7px;  
    height: 7px; 
    transform: translateY(-50%);  
    border-radius: 10px;
  }


</style>
