<template>
  <div>
    <el-row>
      <el-col :span="2">
        <div>
            <a href="/"><img src="../img/logo1.png" class="logo"></a>
        </div>
      </el-col>
      <el-col :span="21">
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
              <el-menu-item index="1-1"> <router-link to="/personaltable">个人级</router-link></el-menu-item>
              <el-menu-item index="1-2">版本级</el-menu-item>
              <el-menu-item index="1-3">流水线</el-menu-item>
            </el-submenu>
          </el-menu>
        </div>
      </el-col>
      <el-col :span="1">
        <div class="h-menu">
          <a href="/" style="border-bottom-color: transparent; color: rgb(170, 170, 170); background-color: #000;font-size: 13px;">帮助</a>
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'webheader',
}
</script>

<style>
.el-menu--popup-bottom-start {
    margin-top: 0px;
}
.el-submenu__title {
    border-left: 1px solid rgb(168, 164, 164);
    border-right: 1px solid rgb(168, 164, 164);
}
.el-menu--popup {
    min-width: 90px;
}
.el-menu-item {
    font-size: 13px;
}
.el-header{
    background-color: #000;
    color: #000;
    text-align: center;
    line-height: 58px;
    padding: 0 0px;
  }

.el-header{
    padding-left:0px;
    line-height: 77px;
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
