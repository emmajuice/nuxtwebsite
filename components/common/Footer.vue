<template>
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
          <img src="../../assets/images/code@2x.png" alt="">
        </div>
      </div>
    </div>
</template>

<script>
    export default {
        name: "Footer"
    }
</script>

<style type="text/css" lang="scss" scoped>
  .foot-container{
    min-height: 320px;
    background: #BFBFBF;
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
