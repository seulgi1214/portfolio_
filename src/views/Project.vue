<template>
  <section>
    <div class="common_container">
      <h3 class="common_title">PROJECT</h3>
      <article>
        <ul class="project_list">
          <li class="item">
            <div class="item_wrap">
              <div class="img">
                <img :src="nyt" alt="뉴욕타임즈 웹 이미지"/>
              </div>
              <div class="contents">
                <h5 class="title">nyt_news</h5>
                <p class="desc">- 뉴욕타임즈 api를 이용한 반응형 웹 구현</p>
                <span class="lang">- HTML, CSS, JS, VUE</span>
                <span class="view"><a href="https://seulgi1214.github.io/nyt_app/" target="_blank"><i class="far fa-hand-point-right"></i>미리보기</a></span>
                <span class="github"><a href="https://github.com/seulgi1214/nyt_app" target="_blank"><i class="fab fa-github-alt"></i>github</a></span>
              </div>
            </div>
          </li>
          <li class="item">
            <div class="item_wrap">
              <div class="img">
                <img :src="kel" alt="켈로그 웹 이미지"/>
              </div>
              <div class="contents">
                <h5 class="title">켈로그 홈페이지</h5>
                <p class="desc">- 반응형 웹 구현</p>
                <span class="lang">- HTML, CSS, JS</span>
                <span class="view"><a href="https://kellogg-s.vercel.app/" target="_blank"><i class="far fa-hand-point-right"></i>미리보기</a></span>
                <span class="github"><a href="https://github.com/seulgi1214/kellogg-s" target="_blank"><i class="fab fa-github-alt"></i>github</a></span>
              </div>
            </div>
          </li>

          <li class="item">
            <div class="item_wrap">
              <div class="img">
                <img :src="pomodoro" alt="pomodoro 이미지"/>
              </div>
              <div class="contents">
                <h5 class="title">pomodoro</h5>
                <p class="desc">- 25분 학습 5분 휴식 학습법 pomodoro를 js로 구현</p>
                <span class="lang">- HTML, CSS, JS</span>
                <span class="view"><a href="https://pomodoro-mu.vercel.app/" target="_blank"><i class="far fa-hand-point-right"></i>미리보기</a></span>
                <span class="github"><a href="https://github.com/seulgi1214/Pomodoro" target="_blank"><i class="fab fa-github-alt"></i>github</a></span>
              </div>
            </div>
          </li>
        </ul>
      </article>
    </div>
  </section>
</template>
<script>
import nyt from '@/assets/img/nyt.png'
import kel from '@/assets/img/kellogg.png'
import pomodoro from '@/assets/img/pomodoro.png'

export default {
  name: '',
  component: {},
  data(){
    return {
      nyt: nyt,
      kel: kel,
      pomodoro: pomodoro
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

.project_list .item {
  padding: 30px 0;
  border-bottom: 1px solid #BD97CB;
  margin-bottom: 30px;
}

.project_list .item:last-child {
  border-bottom: 0

}

.item_wrap {
  display: flex;
}

.img {
  margin-right: 20px;
}

.img img {
  display: block;
  width: 500px;
}

.contents .title {
  font-size: 3rem;
  font-weight: 900;
}

.contents .desc {
  font-size: 1.3rem;
  margin: 2rem 0 ;
}

.contents span {
  display: block;
  margin-bottom: 2rem;
}

.contents .lang {
  font-size: 1.3rem;
}

.contents .view a:hover, .github a:hover {
  color: #af73c5; 
}

.contents .view i, .github i{
  margin-right: 0.5rem
}




</style>