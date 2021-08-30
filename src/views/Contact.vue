<template>
    <section>
    <div class="common_container">
      <h3 class="common_title">CONTACT</h3>
      <div class="intro">
        <div class="intro_img">
          <img :src="profile" alt="소개이미지">
        </div>
        <div class="intro_content">
          <span><i class="fas fa-user"></i>이슬기(LEE SEULGI)</span>
          <span><i class="fas fa-heart"></i>1991.12.14 (만29세)</span>
          <span><i class="fas fa-phone-alt"></i>010-7651-0355</span>
          <span><i class="fas fa-house-user"></i>인천시 계양구 계산동</span>
          <span><i class="fas fa-envelope"></i>leeseulgi1214@gmail.com</span>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import profile from '@/assets/img/profile.jpg'
export default {
  name: 'contact',
  component: {

  },
  data(){
    return {
      profile: profile
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

.common_container .intro {
  display: flex;
  margin-top: 30px;
  align-items: center;
}

.common_container .intro_content span {
  display: block;
  font-size: 1.3rem;
  margin-bottom: 0.5rem;
  font-weight: 500;
}

.common_container .intro_content span i {
  font-size: 1.1rem;
  color: #BD97CB;
  margin-right: 1rem;
}

.common_container .intro_img {
  margin-right: 30px;
}

.common_container .intro_img img{
  width: 200px;
}

</style>