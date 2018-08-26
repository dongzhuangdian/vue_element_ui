<template>
  <div id="app">

    <div class="toper">
      <a href="/" style="margin-left: 13px;"><span style=" font-size: 12px;font-weight: 600;line-height:24px;color: #fff;">mouse</span></a>
      <div class="t-users">
        <a href="https://console.alauda.cn/ap/registernew" target="_blank" style="color: #777; font-size: 12px;padding: 0 10px;">注册</a>|
        <a href="https://console.alauda.cn/ap/login/" target="_blank" style="color: #777; font-size: 12px;padding: 0 3px;">登录</a>
      </div>
    </div>
    <el-container>

        <el-header>
            <webheader></webheader>
        </el-header>

        <el-main>
            <router-view/>
        </el-main>

    </el-container>

  </div>
</template>

<script>
import webheader from "./components/webheader.vue"
export default {
  name: 'App',
  components:{
    webheader,
  }
}
</script>

<style>

  body > .el-container {
    margin-bottom: 40px;
  }
  .el-col-12{
    width: 100%;
  }
 body {
    margin: 0px;
    font-family: arial,"微软雅黑";
  }

  .toper {
    position: relative;
    top: 0;
    height: 23px;
    z-index: 99;
    width: 100%;
    background-color: #393939;
}

 .t-users{
    float: right;
    margin-right: 20px;
    line-height: 15px;
    color: #777;
    position: relative;
    top: 16%;
}

</style>
