<template>
  <div>
      <Nav />
      <main id="contact">
        <div class="contact_container">
          <h3 class="title">Contact</h3>
        </div>
      </main>
      <Footer/>
  </div>
</template>
<script>

import Nav from '@/components/Nav.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'contact',
  component: {
      Nav,
      Footer
  },
  data(){
    return {
      sampleData: ''
    };
  },
  setup() {},
  created() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
<style scoped>

</style>