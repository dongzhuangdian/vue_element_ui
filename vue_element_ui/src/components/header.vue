<template>
  <div id="header">
<!-- <img src="./assets/logo.png"> -->
      <router-view/>
  <div class="toper">
    <a href="/" style="margin-left: 13px;"><span style=" font-size: 12px;font-weight: 600;line-height:24px;color: #fff;">GREEN STRONGER</span></a>
    <div class="t-users">
      <a href="https://console.alauda.cn/ap/registernew" target="_blank" style="color: #777; font-size: 12px;padding: 0 10px;">注册</a>|
      <a href="https://console.alauda.cn/ap/login/" target="_blank" style="color: #777; font-size: 12px;padding: 0 3px;">登录</a>
    </div>
  </div>
  <el-header>
  <el-row>
      <el-col :span="2"><div><a href="/"><img src="./img/logo1.png" class="logo"></a></div></el-col>
      <el-col :span="22">
    <div>
    <el-menu
        :default-active="activeIndex2"
        class="el-menu-demo"
        mode="horizontal"
        @select="handleSelect"
        background-color="#000"
        text-color="#aaa"
        active-text-color="#ffd04b">

        <el-submenu index="1">
          <template slot="title">工作台</template>
          <el-menu-item index="1-1">个人级</el-menu-item>
          <el-menu-item index="1-2">版本级</el-menu-item>
          <el-menu-item index="1-3">流水线</el-menu-item>
        </el-submenu>
      </el-menu>
    </div>
    </el-col>
  </el-row>
</el-header>
  </div>
</template>

<script>
export default {
  name: 'header',
}
</script>

<style>

.el-header, .el-footer {
    background-color: #000;
    color: #000;
    text-align: center;
    line-height: 60px;
    padding: 0 0px;
  }

  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    text-align: center;
    line-height: 500px;
  }

  .el-main {
    background-color: rgb(243, 233, 233);
    color: #333;
    text-align: center;
    line-height: 160px;
  }

  body > .el-container {
    margin-bottom: 40px;
  }
  .el-col-12{
    width: 100%;
  }
  .el-aside{
    text-align: left;
  }
  .el-header{
    padding-left:0px;
    line-height: 77px;
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

.logo {
    max-width:60%;
    max-height:10%;
    line-height: 72px;
}

.logo:hover{
transform:rotateY(360deg);
transition: all 1s ease-in-out;
-webkit-transform:rotateY(360deg); /* Safari 和 Chrome */
-webkit-transition: all 1s ease-in-out;
}
</style>
