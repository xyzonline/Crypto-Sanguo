<template>
  <div class="PackView is-marginless is-clipped">

    <section class="section1">
          <div class="sectionContainer">
              <div class="logo">
                  <img alt="" width="150" srcset="../assets/img/logo.png"/>
              </div>
              <div class="titleNav">
                  <div>
                      <p class="title">以太三国</p>
                      <p class="subtitle">三国题材与区块链融合的策略游戏</p>
                  </div>
                  <br/>
                  <div class="btndiv">
                    <router-link class="button is-medium" :to="{ name: 'Game' }">进入游戏</router-link>
                    <!-- <a class="button is-medium" href="https://cryptosanguo.pro/#/game" target="_blank">进入游戏</a> -->
                  </div>
                  <div class="btndiv">
                    <router-link class="button is-medium" :to="{ name: 'PreSell' }">预售商城</router-link>
                  </div>
                  <div class="btndiv">
                    <!-- <a class="button is-medium" href="http://old.etherwarship.com" style="background-color: transparent; color:white" target="_blank">白皮书</a> -->
                    <router-link class="button is-medium" :to="{ name: 'BP' }" style="background-color: transparent; color:white">白皮书</router-link>
                  </div>
                  <br/>
                  <br/>
                  <br/>
              </div>
          </div>
    </section>

    <br/>

    <section class="section">
      <div class="sec2toptitle">
        <a class="section2title">独一无二的三国英雄卡</a>
      </div>
      <br/>
      <div class="columns">
        <div class="column is-two-thirds">
        <br/>
        <br/>
        <br/>
          <a class="section2content">这是一款基于以太坊区块链的三国题材的策略游戏。<br>1.0版本中具备简易的战斗方式，着重考察玩家对战场局势的掌控与对兵力的调度，之后将引入资源相关的调度。</a>
          <div style="margin: 30px 8px 20px 6px;border-top:1px solid #C0C0C0;"></div>
          <div class="columns">
            <div class="column is-half">
              <a class="sec2subtitle">英雄卡</a>
              <br>
              <a class="sec2subcontent">玩家可使用幸运币抽取独一无二的三国英雄卡。</a>
            </div>
            <div class="column is-half sec2subtitle">
              <a class="sec2subtitle">幸运币</a>
              <br>
              <a class="sec2subcontent">幸运币市场每天都会售卖一枚唯一编号的幸运币。</a>
            </div>
          </div>
        </div>
        <div class="column cardSample">
            <img alt="" srcset="../assets/img/cardsample.png"/>
        </div>
      </div>
    </section>

    <br/>

    <section class="section">
      <div class="sec2toptitle">
        <a class="section2title">独创的区块链抽卡玩法</a>
      </div>
      <br/>
      <div class="columns">
        <div class="column is-one-third">
            <img alt="" srcset="../assets/img/cardwhich.png"/>
        </div>
        <div class="column">
          <a class="sec2subtitle">以太三国创新推出全新的区块链抽卡玩法。</a>
          <br/>
          <br/>
          <br/>
          <a class="sec2subcontent">
          通过抽卡方法获得武将卡，将会是唯一的官方卡牌发售渠道。<br>
          智能卡包中当前包含的卡牌和中奖概率完全公开透明。</a>
          <div class="btndiv">
            <router-link class="button is-medium" :to="{ name: 'PreSell' }">前往抽卡</router-link>
          </div>
        </div>
      </div>
    </section>

    <br/>

    <section class="section">
      <div class="sec2toptitle">
        <a class="section2title">丰富的游戏玩法</a>
        <br/>
        <a class="sec2subtitle">英雄卡不仅仅是一张卡，他们将成为玩家们的武将，为玩家争夺统治领地，扩张势力。</a>
      </div>
      <br/>
      <div class="columns is-multiline is-mobile">
        <div class="column is-one-third-desktop is-one-third-tablet is-12-mobile playContainer" v-for="item in playstyle">
          <img alt="" v-bind:src="'../static/home/'+item.img+'.jpg'"/>
          <br>
          <a class="playTitle">{{ item.title }}</a>
          <br>
          <a class="playContent">{{ item.content }}</a>
        </div>
        <div class="column is-two-third-desktop is-two-third-tablet is-12-mobile zhilingDiv">
          <a class="playTitle">已提供下列指令：</a>
          <br/>
          <a class="playContent">搜寻：有一定概率可以搜寻到武将人才。搜寻到的概率同执行武将的魅力相关。<br>
            出征：对其他玩家的城池发动攻击。战斗胜利的一方有一定概率获得对手的in game 武
            将。<br>
            调度：调度自己的部队。<br>
            撤退：从战斗中撤退到其他城市。<br>
            移动：仅移动自己的武将。<br>
            更多玩法，敬请期待。</a>
        </div>
      </div>
    </section>

    <section>
      <slider class="sliderContainer" animation="normal" height="700px">
        <slider-item>
          <div class="slide slide1">
            <div class="slideContainer">
              <span class="slidetext slidetitle">各路武将 谁与争锋</span>
              <p class="slidetext">在幸运币商店购买幸运币即可抽取随机一位武将。</p>
              <br>
              <div class="btndiv">
                <router-link class="button is-medium" :to="{ name: 'PreSell' }">了解详情</router-link>
              </div>
            </div>
          </div>
        </slider-item>
        <slider-item>
          <div class="slide slide2">
            <div class="slideContainer">
              <span class="slidetext slidetitle">群雄争霸天下</span>
              <p class="slidetext">指挥武将进行对战，争夺城池，一统天下。</p>
              <br>
              <div class="btndiv">
                <router-link class="button is-medium" :to="{ name: 'Game' }">了解详情</router-link>
              </div>
            </div>
          </div>
        </slider-item>
        <slider-item>
          <div class="slide slide3">
            <div class="slideContainer">
              <span class="slidetext slidetitle">更多内容</span>
              <p class="slidetext">敬请期待。</p>
            </div>
          </div>
        </slider-item>
      </slider>
    </section>

    <br/>

  </div>
</template>

<script>
import { Slider, SliderItem } from 'vue-easy-slider'

export default {
  name: 'PackViewNew',
  components: {
    Slider,
    SliderItem
  },
  data() {
    return {
      playstyle: [
        {"title":"城池", "content":"城池是玩家的统治的领地，也是玩家之间争夺的焦点。", "img":"home_1_chengchi"},
        {"title":"武将", "content":"武将具有，统御，武力，智力，内政和魅力五种属性。", "img":"home_2_wujiang"},
        {"title":"势力", "content":"玩家掌握的所有城市的集合。", "img":"home_3_shili"},
        {"title":"战斗", "content":"开始直到某一方战败或者撤退。", "img":"home_4_zhandou"},
        {"title":"预约", "content":"持有武将卡的玩家将可以对城池进行预约。", "img":"home_5_yuyue"},
        {"title":"时点", "content":"玩家发布指令会消耗时点。", "img":"home_6_shidian"},
        {"title":"指令", "content":"指令是玩家影响游戏进程的主要手段。", "img":"home_7_zhiling"},
      ]
    }
  }
}

</script>

<style scoped>
.PackView {
  background-color: #000;
}

/*
  section 1
*/
.section1 {
  background-image: url("../assets/img/homeBG.jpeg");
  background-size: 100%;
  background-repeat: no-repeat;
  background-color: #000;
  @media (max-width: 800px) {
    background-size: cover;
  }
}
.logo {
  text-align: right;
  padding-right: 30px;
  padding-top: 30px;
  @media (max-width: 800px) {
    text-align: center;
    padding-right: 0px;
  }
}
.sectionContainer {
  background-color: #000;
  opacity: 0.7;
}
.titleNav {
  margin-left: 50px;
  @media (max-width: 800px) {
    margin-left: 0px;
    text-align: center;
  }
}
.title {
  font-size: 60px;
  color: #fff;
}
.subtitle {
  color: #fff;
}
.btndiv {
  margin-top: 20px;
  margin-bottom: 20px;
}

/*
  section 2
*/
.section {
  margin-right: 30px;
  margin-left: 30px;
}
.sec2toptitle {
  text-align: center;
}
.section2title {
  font-size: 40px;
  color: #fff;
}
.section2content {
  font-size: 20px;
  color: #fff;
}
.sec2subtitle {
  font-size: 20px;
  color: #fff;
}
.sec2subcontent {
  color: #999
}

/*
  section 4
*/
.playContainer {
  text-align: center;
}
.playTitle {
  font-size: 20px;
  color: #fff;
}
.playContent {
  color: #999;
}
.zhilingDiv {
  border-style: solid;
  border-width: 1px;
  border-color: white;
  padding: 30px;
  margin: 30px;
  @media (max-width: 770px) {
    margin: 0px;
  }
}

/*
  section 5
*/
.sliderContainer {
  width: 100%;
  height: 999px;
}
.slide {
  width: 100%;
  height: 100%;
  background-size: 100%;
  background-repeat: no-repeat;
  background-color: #000;
  display: inline-block;
  vertical-align: middle;
  padding-left: 30px;
}
.slide1 {
  background-image: url("../assets/img/home1.jpeg");
    background-size: cover;
}
.slide2 {
  background-image: url("../assets/img/home2.jpeg");
    background-size: cover;
}
.slide3 {
  background-image: url("../assets/img/home3.jpeg");
    background-size: cover;
}
.slideContainer {
  margin-top: 55px;
  margin-left: 30px;
  padding: 30px;
  width: 80%;
  height: 50%;
  background-color: #ffffff33;
  /*opacity: 0.5;*/
}
.slidetext {
  color: #000;
  font-size: 20px;
}
.slidetitle {
  font-size: 40px;
}
</style>
