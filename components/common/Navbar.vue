<template>
    <div id="wrap" class="hidden-xs-only hidden-sm-only">
      <div id="logo-box">
        <img class="logoImg" src="../../assets/images/logo@2x.png"/>
        <img class="logoName" src="../../assets/images/name@2x.png"/>
      </div>
      <el-menu id="menu-box" :default-active="activeIndex" class="el-menu-demo" mode="horizontal"  @select="handleSelect">
        <el-menu-item index="1">首页</el-menu-item>
        <el-submenu index="2">
          <template slot="title">产品介绍</template>
          <el-menu-item index="2-1">刷脸支付</el-menu-item>
          <el-menu-item index="2-2">App开发</el-menu-item>
        </el-submenu>
        <el-submenu index="3">
          <template slot="title">企业介绍</template>
          <el-menu-item index="3-1">优卓科技</el-menu-item>
          <el-menu-item index="3-2">背篼帮</el-menu-item>
        </el-submenu>
        <el-menu-item index="4">关于我们</el-menu-item>
      </el-menu>
    </div>
</template>

<script>
    export default {
        name: "Navbar",
      data() {
        return {
          activeIndex: 1,
          activeIndex2: '1'
        };
      },
      methods: {
        handleSelect(key, keyPath) {
          console.log(key, keyPath);
        }
      }
    }
</script>

<style type="text/css" lang="scss" scoped>
  #wrap{
    min-width: 1200px;
    margin: 8px auto;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    #logo-box{
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: flex-end;
      width: 20%;
      .logoImg{
        width: 71px;
        height: 66px;
      }
      .logoName{
        width: 122px;
        height: 26px;
        margin-bottom: 10px;
      }
    };
    .el-menu.el-menu--horizontal {
      border-bottom: 0 !important;
    }
    .el-menu--horizontal>.el-menu-item.is-active {
    border-bottom: 4px solid #EA5514;
    color: #333 !important;
    }
    .el-menu--horizontal>.el-submenu.is-active .el-submenu__title {
      border-bottom: 4px solid #EA5514 !important;
      color: #333 !important;
    }
    .el-submenu.is-active .el-submenu__title {
      border-bottom-color: #EA5514;
    }
    .el-menu--horizontal>.el-submenu .el-submenu__title {
      height: 74px !important;
      line-height: 62px !important;
      border-bottom: 2px solid transparent;
      color: #333;
    }
    .el-menu--horizontal>.el-submenu .el-submenu__icon-arrow {
      display: none !important;
    }
  }
</style>
