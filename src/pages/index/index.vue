<template>
  <div class="BigBox">
    <!-- 顶部内容 -->
    <div class="usertop">
      <div class="box">
        <div class="photo">
          <img src="../../../static/tabs/tx.png" alt />
          <p>思创科技</p>
        </div>
        <div class="ico"></div>
      </div>
      <!-- 搜索栏 -->
      <search-bar></search-bar>
      <!-- 轮播图 -->
      <swiper indicator-dots="true" autoplay="true">
        <swiper-item>
          <img src="../../../static/tabs/yangmei.png" alt />
        </swiper-item>
        <swiper-item>
          <img src="../../../static/tabs/yangmei.png" alt />
        </swiper-item>
        <swiper-item>
          <img src="../../../static/tabs/yangmei.png" alt />
        </swiper-item>
      </swiper>
    </div>
    <!-- 中部 -->
    <div class="middle">
      <!-- 每日特价 -->
      <div class="tejia">
        <div class="left">
          <h3>每日特价</h3>
          <span>家纺产业带</span>
          <p>9块9疯抢</p>
        </div>
        <div class="right">
          <h3>每日特价</h3>
          <span>家纺产业带</span>
          <p>9块9疯抢</p>
        </div>
      </div>
      <!-- 图片 -->
      <div class="middle1">
        <img src="../../../static/tabs/100898d5b1f35a6c.png" alt />
        <img src="../../../static/tabs/100898d5b1f35a6c.png" alt />
        <img src="../../../static/tabs/100898d5b1f35a6c.png" alt />
        <img src="../../../static/tabs/100898d5b1f35a6c.png" alt />
      </div>
    </div>
    <!-- 精选部分 -->
    <div class="handpick">
      <!-- 一级分类 -->
      <div class="tophang">
        <div class="active">
          <h4 >精选</h4>
          <p >为你推荐</p>
        </div>
        <div>
          <h4>电器</h4>
          <p>3C家电</p>
        </div>
        <div>
          <h4>电器</h4>
          <p>3C家电</p>
        </div>
        <div>
          <h4>电器</h4>
          <p>3C家电</p>
        </div>
        <div>
          <h4>电器</h4>
          <p>3C家电</p>
        </div>
        <div>
          <h4>电器</h4>
          <p>3C家电</p>
        </div>
      </div>
      <!-- 二级分类 -->
      <div class="bottomhang">
        <div>
           <img src="../../../static/tabs/100898d5b1f35a6c@2x.png" alt="">
           <p>水星家纺羊毛被 舒肤蕾澳洲羊毛抗菌冬被...</p>
           <span>800</span>
        </div>
        <div>
           <img src="../../../static/tabs/100898d5b1f35a6c@2x.png" alt="">
           <p>水星家纺羊毛被 舒肤蕾澳洲羊毛抗菌冬被...</p>
           <span>800</span>
        </div>
        <div>
           <img src="../../../static/tabs/100898d5b1f35a6c@2x.png" alt="">
           <p>水星家纺羊毛被 舒肤蕾澳洲羊毛抗菌冬被...</p>
           <span>800</span>
        </div>
        <div>
           <img src="../../../static/tabs/100898d5b1f35a6c@2x.png" alt="">
           <p>水星家纺羊毛被 舒肤蕾澳洲羊毛抗菌冬被...</p>
           <span>800</span>
        </div>
        
      </div>
    </div>

  </div>
</template>

<script>
import SearchBar from "../../components/searchbar";

export default {
  data() {
    return {
      motto: "Hello miniprograme",
      userInfo: {
        nickName: "mpvue"
      }
    };
  },

  components: {
    SearchBar
  },

  methods: {
    bindViewTap() {
      const url = "../logs/main";
      if (mpvuePlatform === "wx") {
        mpvue.switchTab({ url });
      } else {
        mpvue.navigateTo({ url });
      }
    }
  },

  created() {
    // let app = getApp()
  }
};
</script>

<style scoped lang='less'>
@import "./main.less";
</style>
