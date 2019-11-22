<template>
  <div>
    <div id="wrap" class="hidden-xs-only hidden-sm-only">
      <div id="logo-box">
        <img class="logoImg" src="../assets/images/logo@2x.png"/>
        <img class="logoName" src="../assets/images/name@2x.png"/>
      </div>
      <el-menu id="menu-box" :default-active="activeIndex" class="el-menu-demo" mode="horizontal"  @select="handleSelect">
        <el-menu-item index="1">
          <nuxt-link to="/">首页</nuxt-link>
        </el-menu-item>
        <el-submenu index="2">
          <template slot="title">产品介绍</template>
          <el-menu-item index="2-1">
            <nuxt-link to="/facepay">刷脸支付</nuxt-link>
          </el-menu-item>
          <nuxt-link to="/huichebang">
            <el-menu-item index="2-2">App开发</el-menu-item></nuxt-link>
        </el-submenu>
        <el-submenu index="3">
          <template slot="title">企业介绍</template>
          <el-menu-item index="3-1">优卓科技</el-menu-item>
          <el-menu-item index="3-2">背篼帮</el-menu-item>
        </el-submenu>
        <el-menu-item index="4">关于我们</el-menu-item>
      </el-menu>
    </div>
    <nuxt/>
    <div class="foot-container">
      <div class="foot-box">
        <div class="contactUs">
          <span>联系我们</span>
          <p>Contact US</p>
        </div>
        <div class="foot-items">
          <div class="foot-item">
            <h4>贵州背篼帮科技服务有限公司</h4>
            <ul>
              <li>地址：贵阳市观山湖区，金融城MAX-C座</li>
              <li>电话：0851-8865-6898</li>
              <li>邮编：550081 </li>
              <li>手机：130-3788-3082</li>
              <li>邮箱：384564509@163.com</li>
            </ul>
          </div>
          <div class="foot-item">
            <h4>贵州背篼帮科技服务有限公司</h4>
            <ul>
              <li>地址：贵阳市观山湖区，金融城MAX-C座</li>
              <li>电话：0851-8865-6898</li>
              <li>邮编：550081 </li>
              <li>手机：130-3788-3082</li>
              <li>邮箱：384564509@163.com</li>
            </ul>
          </div>
        </div>
        <div class="Qrcode">
          <img src="../assets/images/code@2x.png" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import Vue from 'vue'
  import ElementUI from 'element-ui'
  import 'element-ui/lib/theme-chalk/index.css'
  Vue.use(ElementUI);
  import 'element-ui/lib/theme-chalk/display.css';
  import * as Navbar from '../components/common/Navbar';
  import * as Footer from '../components/common/Footer';
  export default {
    component:{Navbar,Footer},
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


<style type="text/css" lang="scss">
  html {
    font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }

  *, *:before, *:after {
    box-sizing: border-box;
    margin: 0;
  }

  .button--green {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #3b8070;
    color: #3b8070;
    text-decoration: none;
    padding: 10px 30px;
  }

  .button--green:hover {
    color: #fff;
    background-color: #3b8070;
  }

  .button--grey {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #35495e;
    color: #35495e;
    text-decoration: none;
    padding: 10px 30px;
    margin-left: 15px;
  }

  .button--grey:hover {
    color: #fff;
    background-color: #35495e;
  }
  #wrap {
    width: 1200px;
    margin: 0 auto;
    display: flex;
    flex-direction: row;
    justify-content: space-between;

    #logo-box {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: flex-end;
      width: 20%;

      .logoImg {
        width: 71px;
        height: 66px;
      }

      .logoName {
        width: 122px;
        height: 26px;
        margin-bottom: 10px;
      }

    }
  ;
    .el-menu.el-menu--horizontal {
      border-bottom: 0 !important;
    }

    .el-menu--horizontal > .el-menu-item.is-active {
      border-bottom: 4px solid #EA5514;
      color: #333 !important;
    }

    .el-menu--horizontal > .el-submenu.is-active .el-submenu__title {
      border-bottom: 4px solid #EA5514 !important;
      color: #333 !important;
    }

    .el-submenu.is-active .el-submenu__title {
      border-bottom-color: #EA5514;
    }

    .el-menu--horizontal > .el-submenu .el-submenu__title {
      height: 74px !important;
      line-height: 62px !important;
      border-bottom: 2px solid transparent;
      color: #333;
    }

    .el-menu--horizontal > .el-submenu .el-submenu__icon-arrow {
      display: none !important;
    }
  }
  /*footer*/
  .foot-container{
    min-height: 320px;
    background: #BFBFBF;
    margin-top:10rem;
    position:relative;
    width: 100%;
    bottom: 0;
    display: flex;
    align-items: center;
    .foot-box{
      width: 1200px;
      margin: 0 auto;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      .contactUs{
        width: 180px;
        display: flex;
        flex-direction: column;
      }
      .foot-items{
        width: 840px;
        display: flex;
        flex-direction: row;
        justify-content: space-around;
      };
      .Qrcode{
        width: 180px;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        img{
          width: 161px;
          height: 161px;
        }
      }
    }
  }

</style>
