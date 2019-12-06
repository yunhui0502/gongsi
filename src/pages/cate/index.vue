<template>
  <div>
    <!-- 顶部搜索栏 -->
    <div class="search">
      <div class="search-item">
        <icon type="search" />
        <span>搜索</span>
      </div>
    </div>
    <div class="content">
      <!-- 左侧一级分类 -->
      <div class="left">
        <div class="menu-item active">精选推荐</div>
        <div class="menu-item">女装</div>
        <div class="menu-item">女装</div>
        <div class="menu-item">女装</div>
      </div>
      <!-- 右侧二级和三级分类 -->
      <div class="right">
        <!-- 二级分类 -->
        <div class="brand-item">
          <!-- 二级分类的标题 -->
          <div class="brand-title">常用分类</div>
          <div class="brand-list">
            <!-- 三级分类 -->
            <div class="brand">
              <img src />
              <p></p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SearchBar from "../../components/searchbar";

export default {
  data() {
    return {};
  },
  components: {
    SearchBar
  }
};
</script>

<style scoped lang="less">
@import "./main.less";
</style>