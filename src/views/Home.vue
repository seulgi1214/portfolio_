<template>
  <div>
    <Nav />
    <main id="home">
      <div class="home_container">
        <h3 class="title">About Me</h3>
        <div>

        </div>
      </div>
    </main>
    <Footer/>
  </div>
</template>


<script>

import Nav from '@/components/Nav.vue';
import Footer from '@/components/Footer.vue';


export default {
  name: 'Home',
  components: {
    Nav,
    Footer
  }
}
</script>


 <style scoped>

  .home_container {
    background: #ffffff;
    border-radius: 5px; 
    padding: 30px;
  }

  .title {
    text-align: left; 
    position: relative; 
    padding-left: 15px;
  }

  .title::before {
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