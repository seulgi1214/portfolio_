<template>
  <nav id="nav">
    <div class="container">
      <router-link to="/" style="margin-right: 25px" @click="changeColor(0)" :class="{active: active_el == 0}">
        <div class="home com">
            <i class="fas fa-home"></i>
        </div>
      </router-link>  
      <div class="wrap com">
        <ul class="list">
          <li><router-link to="/project" @click="changeColor(1)" :class="{active: active_el == 1}">PROJECT</router-link></li>
          <li>RESUME</li>
          <li><router-link to="contact" @click="changeColor(3)" :class="{active: active_el == 3}">CONTACT</router-link></li>
        </ul>
        <div class="icons">
          <i class="fab fa-github"></i>
          <i class="fas fa-bold"></i>
        </div>
      </div>
    </div>
  </nav>

</template>



<script>
export default {

  data(){
  return {
    active_el: 0
  }
},
  methods: {
    changeColor(el) {
      this.active_el = el;
    }
  },

}


</script>



<style scoped>
#nav {
  margin: 30px 0;
}

.container { 
  display: flex; 
  font-weight: 600; 
  font-size: 22px; 
}

.com {
  padding: 20px 30px; 
  border-radius: 5px; 
  -webkit-box-shadow: 1px 3px 10px -7px #b2b2b2; 
  box-shadow: 1px 3px 10px -7px #b2b2b2;
  }

.home {
  background: #BD97CB; 
  color: #ffffff; 
  cursor: pointer;

}

.home:hover {
    background: #af73c5; 
    transition: 0.2s ease-in-out;
}

.wrap {
  display: flex; 
  background: #ffffff; 
  width: 100%; 
  justify-content: space-between;
    
}

.list {
  display: flex;
}

.container .wrap .list li, .wrap .icons i {
  cursor: pointer;
  }


.container .wrap .list li:not(last-child), .wrap .icons i:first-child {
  margin-right: 25px;
  }

.active {
  color: #af73c5; 
}

</style>




