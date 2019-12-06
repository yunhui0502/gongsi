<template>
  <div>
    <!-- 头部 -->
    <div class="header">
      <!-- 顶部 -->
      <div class="top-part">
        <span id="top1" class="iconfont icon-daipingjia"></span>
        <span id="top2" class="iconfont icon-daipingjia"></span>
      </div>
      <div class="profile">
        <!-- 获取头像 -->
        <div class="head-img">
          <open-data type="userAvatarUrl"></open-data>
        </div>
        <!-- 昵称 -->
        <open-data type="userNickName"></open-data>
      </div>
      <div class="plus"></div>
    </div>
    <!-- 我的订单 -->
    <div class="order-list">
      <div class="order-title">我的订单</div>
      <div class="order-content">
        <div class="order-item" v-for="item in orders" :key="item.index">
          <span class="iconfont" :class="item.className"></span>
          <p>{{item.text}}</p>
        </div>
      </div>
    </div>
    <!-- 服务 -->
    <div class="service">
        <div class="service-top">
          <div>工具与服务</div>
        </div>
        <div class="service-img">
            <div>
                <img src="../../../static/images/shp.png" alt="">
                <p>常买商品</p>
            </div>
            <div>
                <img src="../../../static/images/shp.png" alt="">
                <p>我的优惠券</p>
            </div>
            <div>
                <img src="../../../static/images/shp.png" alt="">
                <p>我的关注</p>
            </div>
            <div>
                <img src="../../../static/images/shp.png" alt="">
                <p>我的评论</p>
            </div>
            <div>
                <img src="../../../static/images/shp.png" alt="">
                <p>我的地址</p>
            </div>
            <div>
                <img src="../../../static/images/shp.png" alt="">
                <p>我的二维码</p>
            </div>
            <div>
                <img src="../../../static/images/shp.png" alt="">
                <p>联系客服</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      orders: [
        { text: "待付款", className: "icon-daifukuan" },
        { text: "待收货", className: "icon-daishouhuo" },
        { text: "待评价", className: "icon-daipingjia" },
        { text: "退还/售后", className: "icon-shouhou" },
        { text: "我的订单", className: "icon-single" }
      ]
    };
  }
};
</script>

<style scoped lang="less">
@import "main.less";
</style>
