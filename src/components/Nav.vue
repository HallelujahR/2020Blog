<template>

  <el-menu :default-active="activeIndex"
           class="el-menu-demo"
           mode="horizontal"
           style="margin:0 auto;width:1100px;border:none;"
           router
           @select="handleSelect">

    <el-menu-item>
      <img src="@/assets/riveredlogo.png"
           height="35px;"
           style="text-align: center;"
           alt="">
    </el-menu-item>
    <el-menu-item index="/">首页</el-menu-item>
    <el-menu-item index="/photo">摄影</el-menu-item>
    <el-submenu index="3">
      <template slot="title">语言</template>
      <el-menu-item index="3-1">php</el-menu-item>
      <el-menu-item index="3-2">Laravel</el-menu-item>
      <el-menu-item index="3-3">ThinkPhp</el-menu-item>
    </el-submenu>
    <el-menu-item index="/about">关于</el-menu-item>
    <!-- <el-menu-item index="4"
                  disabled>消息中心</el-menu-item> -->
    <el-menu-item index="5"
                  style="float:right;">登陆/注册</el-menu-item>
  </el-menu>

</template>

<script>
export default {

  data () {
    return {
      activeIndex: '1',
      activeIndex2: '1'
    };
  },
  methods: {
    handleSelect (key, keyPath) {
      console.log(key, keyPath);
    }
  }
}
</script>