<template>
  <section>
    <div class="common_container">
      <h3 class="common_title">PROJECT</h3>
      <article>
        <ul class="project_list">
          <li class="item">
            <a href="https://seulgi1214.github.io/nyt_app/" target="_blank">
              <div class="item_wrap">
                <div class="img">
                  <img :src="nyt" alt="뉴욕타임즈 웹 이미지"/>
                </div>
                <div class="desc">
                  <h5>뉴욕타임즈</h5>
                  <p>뉴욕타임즈 api를 이용한 반응형 웹 구현</p>
                  <span>HTML, CSS, JS, VUE</span>
                </div>
              </div>
            </a>
          </li>
        </ul>
      </article>
    </div>
  </section>
</template>
<script>
import nyt from '@/assets/img/nyt.png'
export default {
  name: '',
  component: {},
  data(){
    return {
      nyt: nyt,
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

.item_wrap {
  display: flex;
}

.img img {
  display: block;
  width: 250px;
}
</style>