<template>
    <el-container>
      <el-header>
      <Navbar/>
      </el-header>
      <el-main>
        <Carousel/>
        <CompanyCard/>
        <AboutUs/>
        <EnterPrise/>
      </el-main>
      <el-foooter>
        <Footer/>
      </el-foooter>
    </el-container>
</template>

<script>
import * as otherComponent from '~/components/index'
import * as commonComponent from '~/components/common'
import * as homeComponent from '~/components/home'

import Vue from 'vue';

export default {
  components: {
    ...homeComponent,...commonComponent,...otherComponent
  },

}



</script>

<style type="text/css" lang="scss" scoped>
  *{
    padding:0;
    margin: 0;
  }
  body{
    background: #F5F5F5;
  }
  #wrap{
    max-width: 1200px;
    margin: 9px auto;
  }
  .el-header {
    padding: 0 20px;
    box-sizing: border-box;
    flex-shrink: 0;
    border-bottom: 1px solid #e6e6e6;
    height: 84px !important;
  }
  el-main{
    padding:0 !important;
  }
  el-foooter{
    width: 100%;
  }
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

