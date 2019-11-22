<template>
  <div class="block">
    <el-carousel height="650px">
      <el-carousel-item v-for="item in 4" :key="item">
        <h3 class="small">{{ item }}</h3>
      </el-carousel-item>
    </el-carousel>
    <div class="setupInfo-box">
      <div class="setup-item">
        <span>2016<p>年</p></span>
        <p>背篼帮成立</p>
      </div>
      <el-divider direction="vertical"></el-divider>
      <div class="setup-item">
        <span>2019<p>年</p></span>
        <p>优卓科技成立</p>
      </div>
      <el-divider direction="vertical"></el-divider>
      <div class="setup-item">
        <span>24<p>小时</p></span>
        <p>管家式服务，售后上期稳定无忧</p>
      </div>
      <el-divider direction="vertical"></el-divider>
      <div class="setup-item">
          <span>50
            <ul>
              <li>+</li><li>人</li>
            </ul>
          </span>
        <p>顶尖研发团队+设计团队</p>
      </div>
    </div>
  </div>
</template>
<script>
    export default {
        name: "Carousel"
    }
</script>
<style type="text/css" lang="scss" scoped>
  .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 650px;
    margin: 0;
  }
  el-carousel{
    padding: 0 !important;
  }
  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }
  .el-carousel__indicators--horizontal {
    bottom: 31px;
    left: 50%;
    -webkit-transform: translateX(-50%);
    transform: translateX(-50%);
  }
  .el-divider--vertical {
    display: inline-block;
    width: 2px;
    height: 6em;
    margin: 0 8px;
    vertical-align: middle;
    position: relative;
  }
  .setupInfo-box {
    background: #fff;
    padding: 1rem;
    position: relative;
    top: -2rem;
    z-index: 999;
    display: flex;
    max-width: 1200px;
    margin: 0 auto;
    justify-content: space-around;
    align-items: center;
    box-shadow: 4px 15px 14px 2px #ccc;
    .setup-item{
      span{
        display: flex;
      }
    }
  }
</style>
