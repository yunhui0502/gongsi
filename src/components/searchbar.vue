<template>
  <div class="search">
    <div @click="handleeJump" class="search-item">
      <icon type="search" />
      <span>搜索</span>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    handleeJump () {
    // 控制页面的跳转
    wx.navigateTo({
      url:'#'
    })
  }
  },
};
</script>

<style scoped>
.search {
  background-color: #FF3333;
  padding: 20rpx;
}
.search-item {
 background-color: #fff;
  text-align: center;
  padding: 20rpx;
  margin: 0 20rpx;
  color: #888;
  border-radius: 35rpx;
}
.search .search-item icon {
  vertical-align: middle;
}
</style>
