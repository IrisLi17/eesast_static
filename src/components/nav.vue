<template>
  <div>

    <el-menu
  :default-active="activeIndex2"
  class="el-menu-demo"
  mode="horizontal"
  @select="handleSelect"
  background-color="#545c64"
  text-color="#fff"
  active-text-color="#ffd04b">
  <div class="top">
    <img src="..\..\static\EESAST2017_mini.jpg">
    <div>
      <h2>清华大学电子工程系学生科学技术协会</h2>
      <h3>Student Association of Science and Technology</h3>
    </div>
    
  </div>
  <el-menu-item index="1">首页</el-menu-item>
  <el-submenu index="2">
    <template slot="title">我的工作台</template>
    <el-menu-item index="2-1">选项1</el-menu-item>
    <el-menu-item index="2-2">选项2</el-menu-item>
    <el-menu-item index="2-3">选项3</el-menu-item>
    <el-submenu index="2-4">
      <template slot="title">选项4</template>
      <el-menu-item index="2-4-1">选项1</el-menu-item>
      <el-menu-item index="2-4-2">选项2</el-menu-item>
      <el-menu-item index="2-4-3">选项3</el-menu-item>
    </el-submenu>
  </el-submenu>
  <el-menu-item index="3">消息中心</el-menu-item>
  <el-menu-item index="4"><a href="" target="_blank">订单管理</a></el-menu-item>
  <el-menu-item index="5">注册</el-menu-item>
  <el-menu-item index="6">登录</el-menu-item>
  </el-menu>
  </div>
</template>

<script>
export default {
    name: 'navbar',
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1',
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style scoped>
.top {
    display: flex;
}
.top h2,.top h3{
    margin: auto 0;
    color: white;
}

</style>
